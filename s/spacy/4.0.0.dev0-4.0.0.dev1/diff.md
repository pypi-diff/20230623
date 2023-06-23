# Comparing `tmp/spacy-4.0.0.dev0.tar.gz` & `tmp/spacy-4.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-4.0.0.dev0.tar", last modified: Thu Jan 19 08:47:20 2023, max compression
+gzip compressed data, was "spacy-4.0.0.dev1.tar", last modified: Fri Jun 23 12:19:08 2023, max compression
```

## Comparing `spacy-4.0.0.dev0.tar` & `spacy-4.0.0.dev1.tar`

### file list

```diff
@@ -1,1102 +1,1126 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:20.001715 spacy-4.0.0.dev0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1128 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    22433 2023-01-19 08:47:20.001715 spacy-4.0.0.dev0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    20591 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.833714 spacy-4.0.0.dev0/licenses/
--rw-r--r--   0 vsts      (1001) docker     (122)     6541 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/licenses/3rd_party_licenses.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3242 2023-01-19 08:47:20.001715 spacy-4.0.0.dev0/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     7754 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.841714 spacy-4.0.0.dev0/spacy/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2954 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       80 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      326 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/about.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/attrs.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2664 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/attrs.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.845714 spacy-4.0.0.dev0/spacy/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     1925 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24161 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4845 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/apply.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/assemble.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9401 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/convert.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4546 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/debug_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)    46061 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/debug_data.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3580 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/debug_diff.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8909 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/debug_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/download.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8191 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/evaluate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9379 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/find_threshold.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6403 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/info.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10376 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/init_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5644 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/init_pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21380 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/package.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5141 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/pretrain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3452 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/profile.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.845714 spacy-4.0.0.dev0/spacy/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8208 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/assets.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4754 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/clone.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5138 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/document.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8543 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/dvc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2862 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/pull.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2764 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/push.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8236 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/remote_storage.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15834 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/project/run.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.845714 spacy-4.0.0.dev0/spacy/cli/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)    12928 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/templates/quickstart_training.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     6294 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/templates/quickstart_training_recommendations.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     3399 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/train.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4575 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/cli/validate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1346 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4350 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/default_config.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      738 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/default_config_pretraining.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.845714 spacy-4.0.0.dev0/spacy/displacy/
--rw-r--r--   0 vsts      (1001) docker     (122)    10266 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/displacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23810 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/displacy/render.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4656 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/displacy/templates.py
--rw-r--r--   0 vsts      (1001) docker     (122)    65718 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/errors.py
--rw-r--r--   0 vsts      (1001) docker     (122)       73 2023-01-19 08:46:30.000000 spacy-4.0.0.dev0/spacy/git_info.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13185 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/glossary.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.845714 spacy-4.0.0.dev0/spacy/kb/
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      390 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/candidate.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2606 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/candidate.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      265 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/kb.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     4460 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/kb.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     6797 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/kb_in_memory.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    26431 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/kb/kb_in_memory.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.849714 spacy-4.0.0.dev0/spacy/lang/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.849714 spacy-4.0.0.dev0/spacy/lang/af/
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/af/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/af/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.849714 spacy-4.0.0.dev0/spacy/lang/am/
--rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/am/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/am/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/am/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      544 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/am/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3202 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/am/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/am/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.849714 spacy-4.0.0.dev0/spacy/lang/ar/
--rw-r--r--   0 vsts      (1001) docker     (122)      572 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ar/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ar/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ar/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      460 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ar/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3180 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ar/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1502 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ar/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.849714 spacy-4.0.0.dev0/spacy/lang/az/
--rw-r--r--   0 vsts      (1001) docker     (122)      329 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/az/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      747 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/az/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1697 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/az/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/az/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.849714 spacy-4.0.0.dev0/spacy/lang/bg/
--rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      636 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bg/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2048 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bg/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4748 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bg/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9110 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bg/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.853714 spacy-4.0.0.dev0/spacy/lang/bn/
--rw-r--r--   0 vsts      (1001) docker     (122)     1175 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bn/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1270 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bn/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6156 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bn/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      971 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/bn/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.853714 spacy-4.0.0.dev0/spacy/lang/ca/
--rwxr-xr-x   0 vsts      (1001) docker     (122)     1344 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      595 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      956 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/lex_attrs.py
--rwxr-xr-x   0 vsts      (1001) docker     (122)     1650 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1619 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1994 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/syntax_iterators.py
--rwxr-xr-x   0 vsts      (1001) docker     (122)     1962 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ca/tokenizer_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14678 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/char_classes.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.853714 spacy-4.0.0.dev0/spacy/lang/cs/
--rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/cs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1514 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/cs/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1074 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/cs/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2263 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/cs/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.853714 spacy-4.0.0.dev0/spacy/lang/da/
--rw-r--r--   0 vsts      (1001) docker     (122)      628 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3575 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      912 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1345 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8956 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/da/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.857714 spacy-4.0.0.dev0/spacy/lang/de/
--rw-r--r--   0 vsts      (1001) docker     (122)      616 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/de/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      679 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/de/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1413 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/de/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3661 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/de/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1850 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/de/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5889 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/de/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.857714 spacy-4.0.0.dev0/spacy/lang/dsb/
--rw-r--r--   0 vsts      (1001) docker     (122)      334 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/dsb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      553 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/dsb/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1906 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/dsb/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      118 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/dsb/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.857714 spacy-4.0.0.dev0/spacy/lang/el/
--rw-r--r--   0 vsts      (1001) docker     (122)     1329 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1972 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2086 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/get_pos_from_wiktionary.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2195 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2320 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3411 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8100 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2290 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10077 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/el/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.857714 spacy-4.0.0.dev0/spacy/lang/en/
--rw-r--r--   0 vsts      (1001) docker     (122)     1235 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      556 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1480 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      569 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1570 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14252 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/en/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.861714 spacy-4.0.0.dev0/spacy/lang/es/
--rw-r--r--   0 vsts      (1001) docker     (122)     1288 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      778 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16020 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1796 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3388 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2714 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/es/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.861714 spacy-4.0.0.dev0/spacy/lang/et/
--rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/et/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      246 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/et/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.861714 spacy-4.0.0.dev0/spacy/lang/eu/
--rw-r--r--   0 vsts      (1001) docker     (122)      387 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/eu/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      419 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/eu/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/eu/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)       78 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/eu/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)      760 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/eu/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.861714 spacy-4.0.0.dev0/spacy/lang/fa/
--rw-r--r--   0 vsts      (1001) docker     (122)     1305 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      515 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14856 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/generate_verbs_exc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1386 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      505 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3768 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1555 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    64921 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fa/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.861714 spacy-4.0.0.dev0/spacy/lang/fi/
--rw-r--r--   0 vsts      (1001) docker     (122)      632 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      545 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      857 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6436 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2379 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2468 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fi/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.865714 spacy-4.0.0.dev0/spacy/lang/fr/
--rw-r--r--   0 vsts      (1001) docker     (122)     1404 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)   360608 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/_tokenizer_exceptions_list.py
--rw-r--r--   0 vsts      (1001) docker     (122)      938 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3016 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1627 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1476 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3504 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3124 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11232 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/fr/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.865714 spacy-4.0.0.dev0/spacy/lang/ga/
--rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ga/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4936 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ga/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      608 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ga/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1883 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ga/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.865714 spacy-4.0.0.dev0/spacy/lang/grc/
--rw-r--r--   0 vsts      (1001) docker     (122)      620 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/grc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/grc/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6641 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/grc/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1082 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/grc/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9364 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/grc/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6768 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/grc/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.865714 spacy-4.0.0.dev0/spacy/lang/gu/
--rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/gu/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1215 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/gu/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1004 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/gu/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.865714 spacy-4.0.0.dev0/spacy/lang/he/
--rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/he/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      994 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/he/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1759 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/he/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1856 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/he/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.869714 spacy-4.0.0.dev0/spacy/lang/hi/
--rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1518 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hi/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5889 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hi/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hi/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.869714 spacy-4.0.0.dev0/spacy/lang/hr/
--rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      489 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hr/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)      970 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hr/lemma_lookup_license.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     1999 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hr/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.869714 spacy-4.0.0.dev0/spacy/lang/hsb/
--rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hsb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      640 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hsb/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1791 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hsb/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hsb/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      386 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hsb/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.869714 spacy-4.0.0.dev0/spacy/lang/hu/
--rw-r--r--   0 vsts      (1001) docker     (122)      584 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hu/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      407 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hu/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1491 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hu/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1384 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hu/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8401 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hu/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.869714 spacy-4.0.0.dev0/spacy/lang/hy/
--rw-r--r--   0 vsts      (1001) docker     (122)      317 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hy/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1160 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hy/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1067 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/hy/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.869714 spacy-4.0.0.dev0/spacy/lang/id/
--rw-r--r--   0 vsts      (1001) docker     (122)      698 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    53599 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/_tokenizer_exceptions_list.py
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2139 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6507 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1538 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4205 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/id/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.873714 spacy-4.0.0.dev0/spacy/lang/is/
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/is/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1019 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/is/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.873714 spacy-4.0.0.dev0/spacy/lang/it/
--rw-r--r--   0 vsts      (1001) docker     (122)     1229 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      471 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4615 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      873 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4114 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3137 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1161 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/it/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.873714 spacy-4.0.0.dev0/spacy/lang/ja/
--rw-r--r--   0 vsts      (1001) docker     (122)    12623 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1328 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1639 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/tag_bigram_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3741 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/tag_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ja/tag_orth_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.873714 spacy-4.0.0.dev0/spacy/lang/kn/
--rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/kn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1211 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/kn/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1253 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/kn/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.873714 spacy-4.0.0.dev0/spacy/lang/ko/
--rw-r--r--   0 vsts      (1001) docker     (122)     6887 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ko/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      531 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ko/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1052 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ko/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      268 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ko/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ko/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1928 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ko/tag_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.877714 spacy-4.0.0.dev0/spacy/lang/ky/
--rw-r--r--   0 vsts      (1001) docker     (122)      487 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ky/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      917 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ky/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)      925 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ky/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      848 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ky/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1064 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ky/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2049 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ky/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.877714 spacy-4.0.0.dev0/spacy/lang/la/
--rw-r--r--   0 vsts      (1001) docker     (122)      408 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/la/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      741 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/la/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      619 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/la/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1175 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/la/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.877714 spacy-4.0.0.dev0/spacy/lang/lb/
--rw-r--r--   0 vsts      (1001) docker     (122)      515 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      906 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lb/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1343 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lb/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lb/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1127 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lb/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1168 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lb/tokenizer_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5944 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lex_attrs.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.877714 spacy-4.0.0.dev0/spacy/lang/lg/
--rw-r--r--   0 vsts      (1001) docker     (122)      388 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lg/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2680 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lg/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      569 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lg/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1361 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lg/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.877714 spacy-4.0.0.dev0/spacy/lang/lij/
--rw-r--r--   0 vsts      (1001) docker     (122)      430 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lij/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      397 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lij/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)      270 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lij/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)      853 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lij/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      871 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lij/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/lt/
--rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      602 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lt/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22464 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lt/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      716 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lt/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19708 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lt/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lt/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/lv/
--rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lv/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/lv/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/mk/
--rw-r--r--   0 vsts      (1001) docker     (122)     1689 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1718 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mk/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3468 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mk/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9106 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mk/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3577 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mk/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/ml/
--rw-r--r--   0 vsts      (1001) docker     (122)      321 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ml/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ml/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2345 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ml/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      184 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ml/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/mr/
--rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2456 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/mr/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/nb/
--rw-r--r--   0 vsts      (1001) docker     (122)     1296 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nb/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1663 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nb/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1160 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nb/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1523 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nb/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3069 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nb/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.881714 spacy-4.0.0.dev0/spacy/lang/ne/
--rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ne/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ne/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3276 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ne/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7135 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ne/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.885714 spacy-4.0.0.dev0/spacy/lang/nl/
--rw-r--r--   0 vsts      (1001) docker     (122)     1354 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4618 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1303 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1539 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3090 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2868 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24299 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/nl/tokenizer_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/norm_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.885714 spacy-4.0.0.dev0/spacy/lang/pl/
--rw-r--r--   0 vsts      (1001) docker     (122)     1383 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      685 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pl/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3566 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pl/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1193 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pl/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1362 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pl/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2360 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pl/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.885714 spacy-4.0.0.dev0/spacy/lang/pt/
--rw-r--r--   0 vsts      (1001) docker     (122)      644 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2038 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      456 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2566 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3088 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)      716 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/pt/tokenizer_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/punctuation.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.885714 spacy-4.0.0.dev0/spacy/lang/ro/
--rw-r--r--   0 vsts      (1001) docker     (122)      802 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ro/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      601 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ro/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1680 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ro/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3158 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ro/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2945 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ro/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1461 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ro/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.889715 spacy-4.0.0.dev0/spacy/lang/ru/
--rw-r--r--   0 vsts      (1001) docker     (122)     1317 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ru/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4581 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ru/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7976 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ru/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18734 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ru/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8356 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ru/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25394 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ru/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.889715 spacy-4.0.0.dev0/spacy/lang/sa/
--rw-r--r--   0 vsts      (1001) docker     (122)      317 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sa/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      781 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sa/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4211 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sa/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9364 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sa/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.889715 spacy-4.0.0.dev0/spacy/lang/si/
--rw-r--r--   0 vsts      (1001) docker     (122)      313 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/si/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      944 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/si/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1253 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/si/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2407 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/si/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.889715 spacy-4.0.0.dev0/spacy/lang/sk/
--rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      729 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sk/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1070 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sk/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sk/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.889715 spacy-4.0.0.dev0/spacy/lang/sl/
--rw-r--r--   0 vsts      (1001) docker     (122)      607 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      575 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sl/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6603 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sl/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3274 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sl/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2478 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sl/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13428 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sl/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.889715 spacy-4.0.0.dev0/spacy/lang/sq/
--rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sq/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      467 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sq/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1210 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sq/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.893715 spacy-4.0.0.dev0/spacy/lang/sr/
--rw-r--r--   0 vsts      (1001) docker     (122)      416 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      910 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sr/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1549 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sr/lemma_lookup_licence.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     1426 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sr/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3895 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sr/stop_words.py
--rwxr-xr-x   0 vsts      (1001) docker     (122)     3524 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sr/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.893715 spacy-4.0.0.dev0/spacy/lang/sv/
--rw-r--r--   0 vsts      (1001) docker     (122)     1313 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sv/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sv/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sv/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2545 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sv/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1531 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sv/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3655 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/sv/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.893715 spacy-4.0.0.dev0/spacy/lang/ta/
--rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ta/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ta/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2018 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ta/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.893715 spacy-4.0.0.dev0/spacy/lang/te/
--rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/te/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1243 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/te/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1263 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/te/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1107 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/te/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.897714 spacy-4.0.0.dev0/spacy/lang/th/
--rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/th/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/th/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19463 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/th/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18334 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/th/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.897714 spacy-4.0.0.dev0/spacy/lang/ti/
--rw-r--r--   0 vsts      (1001) docker     (122)      835 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ti/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      821 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ti/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ti/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      545 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ti/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1977 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ti/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      339 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ti/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.897714 spacy-4.0.0.dev0/spacy/lang/tl/
--rw-r--r--   0 vsts      (1001) docker     (122)      416 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      943 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tl/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      965 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tl/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)      688 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tl/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.897714 spacy-4.0.0.dev0/spacy/lang/tn/
--rw-r--r--   0 vsts      (1001) docker     (122)      392 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      436 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tn/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tn/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      588 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tn/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)      816 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tn/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3304 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.901715 spacy-4.0.0.dev0/spacy/lang/tr/
--rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      609 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tr/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tr/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4506 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tr/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1853 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tr/syntax_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6092 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tr/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.901715 spacy-4.0.0.dev0/spacy/lang/tt/
--rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      897 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tt/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tt/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tt/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18567 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tt/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1761 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/tt/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.901715 spacy-4.0.0.dev0/spacy/lang/uk/
--rw-r--r--   0 vsts      (1001) docker     (122)     1332 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/uk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1798 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/uk/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1716 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/uk/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1575 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/uk/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4887 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/uk/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1389 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/uk/tokenizer_exceptions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.905715 spacy-4.0.0.dev0/spacy/lang/ur/
--rw-r--r--   0 vsts      (1001) docker     (122)      461 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ur/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      303 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ur/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2237 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ur/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)       78 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ur/punctuation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4722 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/ur/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.905715 spacy-4.0.0.dev0/spacy/lang/vi/
--rw-r--r--   0 vsts      (1001) docker     (122)     5575 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/vi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      769 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/vi/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1397 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/vi/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20595 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/vi/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.905715 spacy-4.0.0.dev0/spacy/lang/xx/
--rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/xx/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8161 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/xx/examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.905715 spacy-4.0.0.dev0/spacy/lang/yo/
--rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/yo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1269 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/yo/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2523 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/yo/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      608 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/yo/stop_words.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.909715 spacy-4.0.0.dev0/spacy/lang/zh/
--rw-r--r--   0 vsts      (1001) docker     (122)    12738 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/zh/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/zh/examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1613 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/zh/lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13409 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lang/zh/stop_words.py
--rw-r--r--   0 vsts      (1001) docker     (122)   101241 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/language.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2587 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lexeme.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     1411 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lexeme.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    16255 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lexeme.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    10851 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/lookups.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.909715 spacy-4.0.0.dev0/spacy/matcher/
--rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2124 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/dependencymatcher.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    17097 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/dependencymatcher.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)   226181 2023-01-19 08:46:35.000000 spacy-4.0.0.dev0/spacy/matcher/levenshtein.c
--rw-r--r--   0 vsts      (1001) docker     (122)      945 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/levenshtein.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     1530 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/matcher.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     1824 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/matcher.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    49465 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/matcher.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      555 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/phrasematcher.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     1273 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/phrasematcher.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    14701 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/phrasematcher.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     9571 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/matcher/polyleven.c
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.913715 spacy-4.0.0.dev0/spacy/ml/
--rw-r--r--   0 vsts      (1001) docker     (122)      109 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3819 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/callbacks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1993 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/character_embed.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1191 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/extract_ngrams.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2317 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/extract_spans.py
--rw-r--r--   0 vsts      (1001) docker     (122)      969 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/featureextractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.913715 spacy-4.0.0.dev0/spacy/ml/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      224 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3973 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/entity_linker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8745 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/multi_task.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3984 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/parser.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2370 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1252 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/tagger.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6748 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/models/tok2vec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3851 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/staticvectors.py
--rw-r--r--   0 vsts      (1001) docker     (122)      475 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/tb_framework.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    23395 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ml/tb_framework.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     1297 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/morphology.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/morphology.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/parts_of_speech.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      434 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/parts_of_speech.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     6241 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipe_analysis.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.921715 spacy-4.0.0.dev0/spacy/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)     1144 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.921715 spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3449 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/edit_trees.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    10747 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/edit_trees.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     1474 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.925715 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_beam_utils.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    11618 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_beam_utils.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      146 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_parser_utils.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      633 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_parser_utils.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    12621 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_state.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_state.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      211 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/arc_eager.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    30513 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/arc_eager.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/batch.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/batch.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      104 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/ner.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    23467 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/ner.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      187 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/nonproj.hh
--rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/nonproj.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     8603 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/nonproj.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     2652 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/search.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    12326 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/search.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      744 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/stateclass.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     4831 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/stateclass.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     1975 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/transition_system.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    11911 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/transition_system.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    13693 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/attribute_ruler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13081 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/dep_parser.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14817 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/edit_tree_lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30367 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/entity_linker.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/entityruler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6703 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/functions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.925715 spacy-4.0.0.dev0/spacy/pipeline/legacy/
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18808 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/legacy/entity_linker.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12178 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13516 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/morphologizer.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    10150 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/pipe.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     1224 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/pipe.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)     5382 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/pipe.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     6836 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/sentencizer.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     7351 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/senter.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    21727 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/span_ruler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19114 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13982 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/tagger.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    15579 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6910 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/textcat_multilabel.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13389 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/tok2vec.py
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/trainable_pipe.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    17601 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/trainable_pipe.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    31472 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/pipeline/transition_parser.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)    23759 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/schemas.py
--rw-r--r--   0 vsts      (1001) docker     (122)    41002 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/scorer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/strings.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     1226 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/strings.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    11406 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/strings.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     2433 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/structs.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     7063 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/symbols.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    14118 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/symbols.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.929715 spacy-4.0.0.dev0/spacy/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12745 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.933715 spacy-4.0.0.dev0/spacy/tests/doc/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_add_entities.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4988 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_array.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2650 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_creation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    37138 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_doc_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_graph.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13658 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_json_doc_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2993 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_morphanalysis.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1470 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_pickle_doc.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18955 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_retokenize_merge.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10937 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_retokenize_split.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23446 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_span.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7761 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_span_group.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11164 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_token_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10014 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/doc/test_underscore.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.933715 spacy-4.0.0.dev0/spacy/tests/lang/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.933715 spacy-4.0.0.dev0/spacy/tests/lang/af/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/af/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      931 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/af/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      710 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/af/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.933715 spacy-4.0.0.dev0/spacy/tests/lang/am/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/am/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/am/test_exception.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1837 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/am/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.937715 spacy-4.0.0.dev0/spacy/tests/lang/ar/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ar/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      621 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ar/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)      821 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ar/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.937715 spacy-4.0.0.dev0/spacy/tests/lang/bn/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/bn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3623 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/bn/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.937715 spacy-4.0.0.dev0/spacy/tests/lang/ca/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ca/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      621 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ca/test_exception.py
--rw-r--r--   0 vsts      (1001) docker     (122)      493 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ca/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1900 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ca/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.937715 spacy-4.0.0.dev0/spacy/tests/lang/cs/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/cs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      510 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/cs/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.937715 spacy-4.0.0.dev0/spacy/tests/lang/da/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/da/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1824 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/da/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2063 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/da/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/da/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1219 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/da/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.937715 spacy-4.0.0.dev0/spacy/tests/lang/de/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/de/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      598 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/de/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/de/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1188 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/de/test_parser.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3395 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/de/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/de/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.941715 spacy-4.0.0.dev0/spacy/tests/lang/dsb/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/dsb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      560 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/dsb/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      749 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/dsb/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.941715 spacy-4.0.0.dev0/spacy/tests/lang/el/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/el/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      514 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/el/test_exception.py
--rw-r--r--   0 vsts      (1001) docker     (122)      306 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/el/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1768 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/el/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.941715 spacy-4.0.0.dev0/spacy/tests/lang/en/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3798 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_customized_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4158 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)      723 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_indices.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1548 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2954 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_parser.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4254 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4422 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_punct.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1707 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_sbd.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1962 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5938 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/en/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.945715 spacy-4.0.0.dev0/spacy/tests/lang/es/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/es/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      549 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/es/test_exception.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/es/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2025 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/es/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.945715 spacy-4.0.0.dev0/spacy/tests/lang/et/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/et/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      933 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/et/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      737 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/et/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.945715 spacy-4.0.0.dev0/spacy/tests/lang/eu/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/eu/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      488 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/eu/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.945715 spacy-4.0.0.dev0/spacy/tests/lang/fa/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fa/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      296 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fa/test_noun_chunks.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.945715 spacy-4.0.0.dev0/spacy/tests/lang/fi/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7258 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fi/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fi/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2900 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fi/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/fr/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2219 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fr/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8353 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fr/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)      772 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fr/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/fr/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/ga/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ga/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      685 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ga/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/grc/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/grc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/grc/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1327 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/grc/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/gu/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/gu/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      685 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/gu/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/he/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/he/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2255 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/he/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/hi/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1841 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hi/test_lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      400 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hi/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/hr/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hr/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      801 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hr/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.949715 spacy-4.0.0.dev0/spacy/tests/lang/hsb/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hsb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      566 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hsb/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      866 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hsb/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.953715 spacy-4.0.0.dev0/spacy/tests/lang/hu/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hu/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14492 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hu/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.953715 spacy-4.0.0.dev0/spacy/tests/lang/hy/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hy/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1351 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/hy/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.953715 spacy-4.0.0.dev0/spacy/tests/lang/id/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/id/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/id/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3492 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/id/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)      205 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/id/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.953715 spacy-4.0.0.dev0/spacy/tests/lang/is/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/is/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      980 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/is/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      783 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/is/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.953715 spacy-4.0.0.dev0/spacy/tests/lang/it/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/it/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8639 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/it/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/it/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)      449 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/it/test_stopwords.py
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/it/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.957715 spacy-4.0.0.dev0/spacy/tests/lang/ja/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ja/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      694 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ja/test_lemmatization.py
--rw-r--r--   0 vsts      (1001) docker     (122)      243 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ja/test_morphologizer_factory.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1306 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ja/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7900 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ja/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.957715 spacy-4.0.0.dev0/spacy/tests/lang/ko/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ko/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      622 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ko/test_lemmatization.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ko/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4279 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ko/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.957715 spacy-4.0.0.dev0/spacy/tests/lang/ky/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ky/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4014 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ky/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.957715 spacy-4.0.0.dev0/spacy/tests/lang/la/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/la/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      236 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/la/test_exception.py
--rw-r--r--   0 vsts      (1001) docker     (122)      803 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/la/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.957715 spacy-4.0.0.dev0/spacy/tests/lang/lb/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lb/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)      584 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lb/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1302 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lb/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.957715 spacy-4.0.0.dev0/spacy/tests/lang/lg/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lg/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      449 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lg/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/lt/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lt/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/lv/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lv/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1018 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lv/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      778 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/lv/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/mk/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/mk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4352 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/mk/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/ml/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ml/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1075 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ml/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/nb/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/nb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      277 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/nb/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)      630 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/nb/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/ne/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ne/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      783 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ne/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.961715 spacy-4.0.0.dev0/spacy/tests/lang/nl/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/nl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4303 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/nl/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)      693 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/nl/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/pl/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/pl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/pl/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      555 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/pl/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/pt/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/pt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7748 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/pt/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)      219 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/pt/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/ro/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ro/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      734 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ro/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/ru/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ru/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      353 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ru/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3958 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ru/test_lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ru/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5983 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ru/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/sa/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sa/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1297 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sa/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/sk/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1485 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sk/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      453 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sk/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.965715 spacy-4.0.0.dev0/spacy/tests/lang/sl/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      993 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sl/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sl/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.969715 spacy-4.0.0.dev0/spacy/tests/lang/sq/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sq/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1178 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sq/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sq/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.969715 spacy-4.0.0.dev0/spacy/tests/lang/sr/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      510 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sr/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4302 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sr/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.969715 spacy-4.0.0.dev0/spacy/tests/lang/sv/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2453 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)      683 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/test_lex_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1857 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1053 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)      723 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1005 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/sv/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.969715 spacy-4.0.0.dev0/spacy/tests/lang/ta/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2737 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ta/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7829 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ta/test_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3322 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/test_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      922 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/test_initialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1910 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/test_lemmatizers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.973715 spacy-4.0.0.dev0/spacy/tests/lang/th/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/th/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      706 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/th/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/th/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.973715 spacy-4.0.0.dev0/spacy/tests/lang/ti/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ti/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ti/test_exception.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2120 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ti/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.973715 spacy-4.0.0.dev0/spacy/tests/lang/tl/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      257 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tl/test_indices.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4420 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tl/test_punct.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2479 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tl/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.973715 spacy-4.0.0.dev0/spacy/tests/lang/tr/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      422 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tr/test_noun_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19784 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tr/test_parser.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1796 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tr/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19589 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tr/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.973715 spacy-4.0.0.dev0/spacy/tests/lang/tt/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3721 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/tt/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.977715 spacy-4.0.0.dev0/spacy/tests/lang/uk/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/uk/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      837 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/uk/test_lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5416 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/uk/test_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      364 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/uk/test_tokenizer_exc.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.977715 spacy-4.0.0.dev0/spacy/tests/lang/ur/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ur/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ur/test_prefix_suffix_infix.py
--rw-r--r--   0 vsts      (1001) docker     (122)      479 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/ur/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.977715 spacy-4.0.0.dev0/spacy/tests/lang/vi/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/vi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/vi/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1677 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/vi/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.977715 spacy-4.0.0.dev0/spacy/tests/lang/xx/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/xx/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/xx/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)      669 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/xx/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.977715 spacy-4.0.0.dev0/spacy/tests/lang/yo/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/yo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1490 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/yo/test_text.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.981715 spacy-4.0.0.dev0/spacy/tests/lang/zh/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/zh/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1245 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/zh/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/zh/test_text.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2819 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/lang/zh/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.981715 spacy-4.0.0.dev0/spacy/tests/matcher/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14304 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/test_dependency_matcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2797 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/test_levenshtein.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30055 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/test_matcher_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)    27183 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/test_matcher_logic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3334 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/test_pattern_validation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17364 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/matcher/test_phrase_matcher.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.985715 spacy-4.0.0.dev0/spacy/tests/morphology/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/morphology/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      856 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/morphology/test_morph_converters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1348 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/morphology/test_morph_features.py
--rw-r--r--   0 vsts      (1001) docker     (122)      668 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/morphology/test_morph_pickle.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.985715 spacy-4.0.0.dev0/spacy/tests/package/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/package/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-01-19 08:46:30.000000 spacy-4.0.0.dev0/spacy/tests/package/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)      992 2023-01-19 08:46:30.000000 spacy-4.0.0.dev0/spacy/tests/package/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3523 2023-01-19 08:46:30.000000 spacy-4.0.0.dev0/spacy/tests/package/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     3151 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/package/test_requirements.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.989715 spacy-4.0.0.dev0/spacy/tests/parser/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3148 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/_search.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     4919 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_add_label.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10085 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_arc_eager_oracle.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30390 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2859 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_neural_parser.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3600 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_nn_beam.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6289 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_nonproj.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23784 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_parse.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_parse_navigate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2560 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_preset_sbd.py
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_search.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2927 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_space_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1894 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/parser/test_state.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.989715 spacy-4.0.0.dev0/spacy/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3456 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_analysis.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3192 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_annotates_on_update.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9535 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_attributeruler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12043 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_edit_tree_lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    47651 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_entity_linker.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20789 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_entity_ruler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3188 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_functions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2350 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_initialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3725 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_lemmatizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3842 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8088 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_morphologizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19895 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_pipe_factories.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23041 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_pipe_methods.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18273 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_sentencizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4294 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_senter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16221 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_span_ruler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15962 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8887 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_tagger.py
--rw-r--r--   0 vsts      (1001) docker     (122)    37365 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18811 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/pipeline/test_tok2vec.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.993715 spacy-4.0.0.dev0/spacy/tests/serialize/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4185 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_resource_warning.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16025 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_config.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6931 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_doc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3687 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_docbin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      945 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_extension_attrs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_kb.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3594 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_language.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15013 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8766 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_span_groups.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7067 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_vocab_strings.py
--rw-r--r--   0 vsts      (1001) docker     (122)      447 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)    43308 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1203 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12974 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_displacy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_errors.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26991 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_language.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13415 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_misc.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9089 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_models.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2022 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_pickles.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16857 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_scorer.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10600 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_symbols.py
--rw-r--r--   0 vsts      (1001) docker     (122)      748 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/test_ty.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.993715 spacy-4.0.0.dev0/spacy/tests/tokenizer/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2591 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/sun.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     1756 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/test_explain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7466 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/test_naughty_strings.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18589 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/test_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6605 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/test_urls.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1295 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/tokenizer/test_whitespace.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.993715 spacy-4.0.0.dev0/spacy/tests/training/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10607 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_augmenters.py
--rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_logger.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16145 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_new_example.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10842 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_pretraining.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3947 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_readers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6405 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_rehearse.py
--rw-r--r--   0 vsts      (1001) docker     (122)    46167 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/training/test_training.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3204 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.993715 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2852 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_lexeme.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4651 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_lookups.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3834 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_similarity.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3939 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_stringstore.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22581 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_vectors.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2147 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_vocab_api.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2158 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokenizer.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    36322 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokenizer.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.997715 spacy-4.0.0.dev0/spacy/tokens/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      248 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1667 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/doc.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     5947 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/doc.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    83730 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/doc.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    11891 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/doc_bin.py
--rw-r--r--   0 vsts      (1001) docker     (122)      295 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/graph.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    23114 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/graph.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      303 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/morphanalysis.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      820 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/morphanalysis.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)     2941 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/morphanalysis.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      702 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/retokenizer.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    20452 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/retokenizer.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      632 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     3821 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    34475 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      307 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span_group.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      835 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span_group.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    11137 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span_group.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     4515 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/span_groups.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3419 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/token.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     5346 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/token.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    33015 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/token.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     6926 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/tokens/underscore.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:20.001715 spacy-4.0.0.dev0/spacy/training/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)      880 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/align.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      614 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/alignment.py
--rw-r--r--   0 vsts      (1001) docker     (122)      170 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/alignment_array.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2128 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/alignment_array.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    13279 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/augment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9446 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/batchers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1267 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/callbacks.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:20.001715 spacy-4.0.0.dev0/spacy/training/converters/
--rw-r--r--   0 vsts      (1001) docker     (122)      224 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/converters/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6177 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/converters/conll_ner_to_docs.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10275 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/converters/conllu_to_docs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2356 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/converters/iob_to_docs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      883 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/converters/json_to_docs.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9323 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/corpus.py
--rw-r--r--   0 vsts      (1001) docker     (122)      327 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/example.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)    25036 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/example.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     8027 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/gold_io.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    13716 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/initialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9075 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/iob_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7819 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/loggers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15059 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/loop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9356 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/training/pretrain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)      283 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/typedefs.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/typedefs.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)    65665 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)    25940 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/vectors.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     1305 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/vocab.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     2727 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/vocab.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)    23180 2023-01-19 08:46:07.000000 spacy-4.0.0.dev0/spacy/vocab.pyx
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-19 08:47:19.841714 spacy-4.0.0.dev0/spacy.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    22433 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    29202 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-01-19 08:47:19.000000 spacy-4.0.0.dev0/spacy.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.324712 spacy-4.0.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1128 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    16877 2023-06-23 12:19:08.324712 spacy-4.0.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    15135 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.184711 spacy-4.0.0.dev1/licenses/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6541 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/licenses/3rd_party_licenses.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3261 2023-06-23 12:19:08.324712 spacy-4.0.0.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     7754 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.192711 spacy-4.0.0.dev1/spacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     2954 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       80 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      326 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/about.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/attrs.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     2664 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/attrs.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.192711 spacy-4.0.0.dev1/spacy/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1988 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24798 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4845 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/apply.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2574 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/assemble.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5217 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/benchmark_speed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9527 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/convert.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4546 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/debug_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    50096 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/debug_data.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3580 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/debug_diff.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8909 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/debug_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4711 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/download.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9287 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/evaluate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9380 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/find_threshold.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6329 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/info.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10899 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/init_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5626 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/init_pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21385 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/package.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5260 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/pretrain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3452 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/profile.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.196711 spacy-4.0.0.dev1/spacy/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8208 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/assets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4754 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5138 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8543 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/dvc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2942 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/pull.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2774 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/push.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8236 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/remote_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15838 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/project/run.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.196711 spacy-4.0.0.dev1/spacy/cli/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16206 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/templates/quickstart_training.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     6294 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/cli/templates/quickstart_training_recommendations.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3399 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/train.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4575 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/cli/validate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      727 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4350 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/default_config.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      559 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/default_config_distillation.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      738 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/default_config_pretraining.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.196711 spacy-4.0.0.dev1/spacy/displacy/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10356 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/displacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23810 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/displacy/render.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4656 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/displacy/templates.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    67123 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       73 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy/git_info.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13185 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/glossary.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.196711 spacy-4.0.0.dev1/spacy/kb/
+-rw-r--r--   0 vsts      (1001) docker     (122)      208 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      392 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/candidate.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     3325 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/candidate.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      265 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/kb.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5059 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/kb.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     6797 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/kb_in_memory.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    26570 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/kb/kb_in_memory.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.196711 spacy-4.0.0.dev1/spacy/lang/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.196711 spacy-4.0.0.dev1/spacy/lang/af/
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/af/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/af/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/am/
+-rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/am/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/am/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/am/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      544 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/am/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3202 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/am/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/am/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/ar/
+-rw-r--r--   0 vsts      (1001) docker     (122)      572 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ar/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      890 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ar/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ar/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      460 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ar/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3180 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ar/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1502 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ar/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/az/
+-rw-r--r--   0 vsts      (1001) docker     (122)      329 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/az/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      747 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/az/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1697 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/az/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/az/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/bg/
+-rw-r--r--   0 vsts      (1001) docker     (122)      919 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/bg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      636 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/bg/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2048 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/bg/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4748 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/bg/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9110 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/bg/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/bn/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1175 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/bn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/bn/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1270 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/bn/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6156 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/bn/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      971 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/bn/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/ca/
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1344 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ca/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      595 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ca/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2843 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ca/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      956 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ca/lex_attrs.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1650 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ca/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1619 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ca/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1994 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ca/syntax_iterators.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     1962 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ca/tokenizer_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14678 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/char_classes.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.200711 spacy-4.0.0.dev1/spacy/lang/cs/
+-rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/cs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1514 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/cs/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1074 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/cs/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2263 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/cs/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.204711 spacy-4.0.0.dev1/spacy/lang/da/
+-rw-r--r--   0 vsts      (1001) docker     (122)      628 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/da/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/da/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3575 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/da/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      912 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/da/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1345 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/da/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2188 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/da/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8956 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/da/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.204711 spacy-4.0.0.dev1/spacy/lang/de/
+-rw-r--r--   0 vsts      (1001) docker     (122)      616 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/de/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      679 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/de/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1413 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/de/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3661 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/de/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1850 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/de/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5889 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/de/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.204711 spacy-4.0.0.dev1/spacy/lang/dsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)      334 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/dsb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      553 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/dsb/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1906 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/dsb/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      118 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/dsb/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.204711 spacy-4.0.0.dev1/spacy/lang/el/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1329 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/el/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1972 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/el/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2086 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/el/get_pos_from_wiktionary.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2195 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/el/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2320 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/el/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3411 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/el/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8100 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/el/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2290 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/el/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10077 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/el/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.204711 spacy-4.0.0.dev1/spacy/lang/en/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1235 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/en/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      556 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/en/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1480 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/en/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/en/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      569 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/en/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/en/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1570 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/en/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14252 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/en/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.208711 spacy-4.0.0.dev1/spacy/lang/es/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1288 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/es/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      778 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/es/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16020 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/es/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1796 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/es/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1234 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/es/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3388 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/es/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2714 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/es/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1458 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/es/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.208711 spacy-4.0.0.dev1/spacy/lang/et/
+-rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/et/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      246 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/et/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.208711 spacy-4.0.0.dev1/spacy/lang/eu/
+-rw-r--r--   0 vsts      (1001) docker     (122)      387 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/eu/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      419 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/eu/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/eu/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       78 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/eu/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      760 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/eu/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.208711 spacy-4.0.0.dev1/spacy/lang/fa/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1305 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fa/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      515 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fa/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14856 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fa/generate_verbs_exc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1386 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fa/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      505 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fa/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3768 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fa/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1555 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fa/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    64921 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fa/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.208711 spacy-4.0.0.dev1/spacy/lang/fi/
+-rw-r--r--   0 vsts      (1001) docker     (122)      632 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      545 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fi/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fi/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      857 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fi/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6436 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fi/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2379 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fi/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2468 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fi/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/fr/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1404 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   360608 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fr/_tokenizer_exceptions_list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      938 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fr/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3016 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fr/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1627 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fr/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1476 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fr/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3504 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/fr/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3124 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fr/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11232 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/fr/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/ga/
+-rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ga/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4936 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ga/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      608 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ga/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1883 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ga/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/grc/
+-rw-r--r--   0 vsts      (1001) docker     (122)      620 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/grc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/grc/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6641 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/grc/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1082 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/grc/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9364 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/grc/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6768 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/grc/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/gu/
+-rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/gu/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1215 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/gu/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1004 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/gu/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/he/
+-rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/he/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      994 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/he/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1759 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/he/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1856 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/he/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/hi/
+-rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1518 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hi/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5889 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hi/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hi/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.212711 spacy-4.0.0.dev1/spacy/lang/hr/
+-rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      489 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hr/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      970 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hr/lemma_lookup_license.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1999 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hr/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.216711 spacy-4.0.0.dev1/spacy/lang/hsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hsb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      640 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hsb/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1791 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hsb/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hsb/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      386 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hsb/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.216711 spacy-4.0.0.dev1/spacy/lang/hu/
+-rw-r--r--   0 vsts      (1001) docker     (122)      584 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hu/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      407 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hu/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1491 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hu/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1384 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hu/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8401 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hu/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.216711 spacy-4.0.0.dev1/spacy/lang/hy/
+-rw-r--r--   0 vsts      (1001) docker     (122)      317 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hy/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1160 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/hy/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1067 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/hy/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.216711 spacy-4.0.0.dev1/spacy/lang/id/
+-rw-r--r--   0 vsts      (1001) docker     (122)      698 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/id/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    53599 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/id/_tokenizer_exceptions_list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/id/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1277 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/id/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2139 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/id/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6507 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/id/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1538 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/id/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4205 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/id/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.216711 spacy-4.0.0.dev1/spacy/lang/isl/
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/isl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1019 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/isl/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.216711 spacy-4.0.0.dev1/spacy/lang/it/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1229 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/it/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      471 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/it/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4615 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/it/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      873 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/it/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4114 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/it/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3137 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/it/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1161 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/it/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.220711 spacy-4.0.0.dev1/spacy/lang/ja/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12623 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ja/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ja/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1328 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ja/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1639 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ja/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1647 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ja/tag_bigram_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3741 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ja/tag_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ja/tag_orth_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.220711 spacy-4.0.0.dev1/spacy/lang/kn/
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/kn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1211 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/kn/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1253 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/kn/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.220711 spacy-4.0.0.dev1/spacy/lang/ko/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6887 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ko/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      531 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ko/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1052 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ko/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      268 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ko/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ko/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1928 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ko/tag_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.220711 spacy-4.0.0.dev1/spacy/lang/ky/
+-rw-r--r--   0 vsts      (1001) docker     (122)      487 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ky/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      917 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ky/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      925 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ky/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      848 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ky/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1064 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ky/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2049 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ky/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.220711 spacy-4.0.0.dev1/spacy/lang/la/
+-rw-r--r--   0 vsts      (1001) docker     (122)      495 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/la/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1146 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/la/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2371 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/la/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      619 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/la/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2391 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/la/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1236 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/la/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.220711 spacy-4.0.0.dev1/spacy/lang/lb/
+-rw-r--r--   0 vsts      (1001) docker     (122)      515 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      906 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lb/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1343 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lb/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      641 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lb/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1127 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lb/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1168 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lb/tokenizer_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5944 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lex_attrs.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/lg/
+-rw-r--r--   0 vsts      (1001) docker     (122)      388 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lg/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2680 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lg/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      569 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lg/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1361 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lg/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/lij/
+-rw-r--r--   0 vsts      (1001) docker     (122)      430 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lij/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      397 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lij/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      270 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lij/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      853 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lij/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      871 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lij/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/lt/
+-rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      602 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lt/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22464 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lt/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      716 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lt/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19708 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lt/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lt/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/lv/
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/lv/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1085 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/lv/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/mk/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1689 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/mk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1718 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/mk/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3468 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/mk/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9106 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/mk/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3577 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/mk/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/ml/
+-rw-r--r--   0 vsts      (1001) docker     (122)      321 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ml/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2345 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ml/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      184 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ml/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.224711 spacy-4.0.0.dev1/spacy/lang/mr/
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/mr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2456 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/mr/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/ms/
+-rw-r--r--   0 vsts      (1001) docker     (122)      678 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ms/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    27445 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ms/_tokenizer_exceptions_list.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      680 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ms/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1266 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ms/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2135 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ms/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6507 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ms/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1538 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ms/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19110 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ms/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/mul/
+-rw-r--r--   0 vsts      (1001) docker     (122)      268 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/mul/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8161 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/mul/examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/nb/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1296 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      428 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/nb/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1663 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nb/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1160 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/nb/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1523 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nb/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3069 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nb/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/ne/
+-rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ne/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ne/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3276 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ne/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7135 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ne/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/nl/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1354 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/nl/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4618 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/nl/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1303 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nl/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1539 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nl/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3090 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/nl/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2868 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nl/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24299 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/nl/tokenizer_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/norm_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/pl/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1383 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      685 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/pl/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3566 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pl/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1193 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pl/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1362 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pl/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2360 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/pl/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.228711 spacy-4.0.0.dev1/spacy/lang/pt/
+-rw-r--r--   0 vsts      (1001) docker     (122)      644 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/pt/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2038 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pt/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      456 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pt/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2566 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/pt/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3088 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pt/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      716 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/pt/tokenizer_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/punctuation.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.232711 spacy-4.0.0.dev1/spacy/lang/ro/
+-rw-r--r--   0 vsts      (1001) docker     (122)      802 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ro/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      601 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ro/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1680 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ro/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3158 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ro/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2945 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ro/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1461 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ro/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.232711 spacy-4.0.0.dev1/spacy/lang/ru/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1317 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ru/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4581 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ru/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7976 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ru/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18734 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ru/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8356 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ru/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25394 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ru/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.232711 spacy-4.0.0.dev1/spacy/lang/sa/
+-rw-r--r--   0 vsts      (1001) docker     (122)      317 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sa/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      781 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sa/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4211 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sa/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9364 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sa/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.232711 spacy-4.0.0.dev1/spacy/lang/si/
+-rw-r--r--   0 vsts      (1001) docker     (122)      313 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/si/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      944 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/si/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1253 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/si/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2407 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/si/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.232711 spacy-4.0.0.dev1/spacy/lang/sk/
+-rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      729 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sk/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1070 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sk/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sk/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.232711 spacy-4.0.0.dev1/spacy/lang/sl/
+-rw-r--r--   0 vsts      (1001) docker     (122)      607 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      575 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sl/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6603 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sl/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3274 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sl/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2478 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sl/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13428 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sl/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/sq/
+-rw-r--r--   0 vsts      (1001) docker     (122)      251 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sq/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      467 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sq/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1210 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sq/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/sr/
+-rw-r--r--   0 vsts      (1001) docker     (122)      545 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      910 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sr/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1549 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sr/lemma_lookup_licence.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1426 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sr/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      964 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sr/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3895 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sr/stop_words.py
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     3524 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sr/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/sv/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1274 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sv/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sv/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sv/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1023 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sv/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2545 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/sv/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1531 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sv/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3655 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/sv/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/ta/
+-rw-r--r--   0 vsts      (1001) docker     (122)      305 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ta/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ta/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2018 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ta/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/te/
+-rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/te/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1243 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/te/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1263 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/te/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1107 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/te/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/th/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/th/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/th/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19463 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/th/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18334 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/th/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.236711 spacy-4.0.0.dev1/spacy/lang/ti/
+-rw-r--r--   0 vsts      (1001) docker     (122)      835 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ti/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      821 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ti/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ti/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      545 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ti/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1977 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ti/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      339 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ti/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.240712 spacy-4.0.0.dev1/spacy/lang/tl/
+-rw-r--r--   0 vsts      (1001) docker     (122)      416 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      943 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tl/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      965 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tl/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      688 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tl/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.240712 spacy-4.0.0.dev1/spacy/lang/tn/
+-rw-r--r--   0 vsts      (1001) docker     (122)      392 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      436 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tn/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tn/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      588 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tn/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      816 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tn/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3304 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.240712 spacy-4.0.0.dev1/spacy/lang/tr/
+-rw-r--r--   0 vsts      (1001) docker     (122)      546 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      609 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tr/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1674 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tr/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4506 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tr/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1853 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tr/syntax_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6092 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tr/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.240712 spacy-4.0.0.dev1/spacy/lang/tt/
+-rw-r--r--   0 vsts      (1001) docker     (122)      483 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      897 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tt/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tt/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tt/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18567 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/tt/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1761 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/tt/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.240712 spacy-4.0.0.dev1/spacy/lang/uk/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1332 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/uk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1798 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/uk/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1716 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/uk/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1575 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/uk/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4887 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/uk/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1389 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/uk/tokenizer_exceptions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.240712 spacy-4.0.0.dev1/spacy/lang/ur/
+-rw-r--r--   0 vsts      (1001) docker     (122)      461 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ur/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      303 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ur/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2237 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ur/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       78 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/ur/punctuation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4722 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/ur/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.244711 spacy-4.0.0.dev1/spacy/lang/vi/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5575 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/vi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      769 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/vi/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1397 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/vi/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20595 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/vi/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.244711 spacy-4.0.0.dev1/spacy/lang/yo/
+-rw-r--r--   0 vsts      (1001) docker     (122)      309 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/yo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1269 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/yo/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2523 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/yo/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      608 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/yo/stop_words.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.244711 spacy-4.0.0.dev1/spacy/lang/zh/
+-rw-r--r--   0 vsts      (1001) docker     (122)    12738 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/zh/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/zh/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1613 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lang/zh/lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13409 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/lang/zh/stop_words.py
+-rw-r--r--   0 vsts      (1001) docker     (122)   106987 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/language.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2587 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lexeme.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lexeme.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    16247 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lexeme.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    10851 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/lookups.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.244711 spacy-4.0.0.dev1/spacy/matcher/
+-rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2124 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/dependencymatcher.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    17833 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/dependencymatcher.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)   227651 2023-06-23 12:18:19.000000 spacy-4.0.0.dev1/spacy/matcher/levenshtein.c
+-rw-r--r--   0 vsts      (1001) docker     (122)      945 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/matcher/levenshtein.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     1530 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/matcher.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     1826 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/matcher.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    49615 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/matcher.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      555 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/phrasematcher.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     1271 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/phrasematcher.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    14701 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/matcher/phrasematcher.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     9571 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/matcher/polyleven.c
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.244711 spacy-4.0.0.dev1/spacy/ml/
+-rw-r--r--   0 vsts      (1001) docker     (122)      109 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/ml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3819 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/callbacks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1993 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/character_embed.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1191 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/extract_ngrams.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2303 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/extract_spans.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      969 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/featureextractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.248711 spacy-4.0.0.dev1/spacy/ml/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      259 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/ml/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5101 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/entity_linker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9260 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/multi_task.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3963 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/parser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1231 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/span_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2370 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1252 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/tagger.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6748 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14020 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/models/tok2vec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3851 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/staticvectors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      475 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/tb_framework.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    23618 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ml/tb_framework.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     1297 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/morphology.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     9560 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/morphology.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/parts_of_speech.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      434 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/parts_of_speech.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     6241 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipe_analysis.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.252712 spacy-4.0.0.dev1/spacy/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1198 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.252712 spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3449 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/edit_trees.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    10747 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/edit_trees.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     1474 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.252712 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_beam_utils.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    11618 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_beam_utils.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      146 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_parser_utils.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      633 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_parser_utils.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    12621 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_state.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_state.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      211 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/arc_eager.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    30513 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/arc_eager.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/batch.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     1299 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/batch.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      104 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/ner.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    23467 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/ner.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      187 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/nonproj.hh
+-rw-r--r--   0 vsts      (1001) docker     (122)      133 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/nonproj.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     8603 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/nonproj.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     2652 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/search.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    12326 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/search.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      744 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/stateclass.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4831 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/stateclass.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     1975 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/transition_system.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    11911 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/transition_system.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    13693 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/attribute_ruler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13081 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/dep_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17173 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/edit_tree_lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31020 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/entity_linker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/entityruler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6703 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12178 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13930 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/morphologizer.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    10175 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/pipeline/pipe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     1224 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/pipe.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)     5382 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/pipe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     6852 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/sentencizer.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     7368 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/senter.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    12281 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/span_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21727 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/span_ruler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31169 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14317 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/tagger.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    15579 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6910 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/textcat_multilabel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15784 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/tok2vec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/trainable_pipe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    17621 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/trainable_pipe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    33732 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/pipeline/transition_parser.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)    24812 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/schemas.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    41434 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/scorer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      726 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/strings.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     1233 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/strings.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    11406 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/strings.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     2433 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/structs.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     7063 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/symbols.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    14118 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/symbols.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.256712 spacy-4.0.0.dev1/spacy/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12849 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.256712 spacy-4.0.0.dev1/spacy/tests/doc/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/doc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_add_entities.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4988 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_array.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2650 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_creation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    37139 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_doc_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1819 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13658 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_json_doc_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3145 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_morphanalysis.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1470 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_pickle_doc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18955 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_retokenize_merge.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10937 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_retokenize_split.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26883 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_span.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8742 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_span_group.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11164 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_token_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10014 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/doc/test_underscore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.256712 spacy-4.0.0.dev1/spacy/tests/lang/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/af/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/af/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      931 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/af/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      710 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/af/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/am/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/am/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/am/test_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1837 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/am/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/ar/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ar/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      621 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ar/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      821 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ar/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/bn/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/bn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3623 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/bn/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/ca/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ca/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      621 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ca/test_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      493 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ca/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1900 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ca/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/cs/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/cs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      510 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/cs/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/da/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/da/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1824 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/da/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2063 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/da/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5423 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/da/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1219 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/da/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/de/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/de/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      598 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/de/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/de/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1188 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/de/test_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3395 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/de/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1505 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/de/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/dsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/dsb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      560 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/dsb/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      749 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/dsb/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.260712 spacy-4.0.0.dev1/spacy/tests/lang/el/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/el/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      514 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/el/test_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      306 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/el/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1768 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/el/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/en/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3798 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_customized_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4158 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      723 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_indices.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1548 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2954 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4254 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4422 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_punct.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1707 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_sbd.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1962 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5938 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/en/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/es/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/es/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      549 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/es/test_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/es/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2025 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/es/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/et/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/et/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      933 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/et/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      737 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/et/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/eu/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/eu/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      488 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/eu/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/fa/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/fa/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      296 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/fa/test_noun_chunks.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/fi/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/fi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7258 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/fi/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/fi/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2900 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/fi/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/fr/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/fr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2219 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/fr/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8353 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/fr/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      772 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/fr/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/fr/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.264712 spacy-4.0.0.dev1/spacy/tests/lang/ga/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ga/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      685 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ga/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/grc/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/grc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      543 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/grc/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1327 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/grc/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/gu/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/gu/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      685 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/gu/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/he/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/he/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2255 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/he/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/hi/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1841 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/hi/test_lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      400 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/hi/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/hr/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      954 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hr/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      801 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hr/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/hsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hsb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      566 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hsb/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      866 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hsb/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/hu/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hu/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14492 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/hu/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/hy/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/hy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/hy/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1351 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/hy/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/id/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/id/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/id/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3492 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/id/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      205 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/id/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/isl/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/isl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      984 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/isl/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      788 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/isl/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.268712 spacy-4.0.0.dev1/spacy/tests/lang/it/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/it/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8639 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/it/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/it/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      449 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/it/test_stopwords.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/it/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/ja/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ja/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      694 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ja/test_lemmatization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      243 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ja/test_morphologizer_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1306 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ja/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7900 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ja/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/ko/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ko/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      622 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ko/test_lemmatization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ko/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4279 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ko/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/ky/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ky/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4014 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ky/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/la/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/la/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      236 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/la/test_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1627 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/la/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      803 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/la/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/lb/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lb/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      584 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lb/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1302 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lb/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/lg/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lg/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      449 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lg/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/lt/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lt/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/lv/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lv/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1018 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lv/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      778 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/lv/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/mk/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/mk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4352 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/mk/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/ml/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1075 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ml/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/ms/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ms/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ms/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3512 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ms/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      205 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ms/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.272712 spacy-4.0.0.dev1/spacy/tests/lang/mul/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/mul/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1722 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/mul/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      674 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/mul/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/nb/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/nb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      277 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/nb/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      630 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/nb/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/ne/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ne/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      783 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ne/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/nl/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/nl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4303 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/nl/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      693 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/nl/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/pl/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/pl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      522 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/pl/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      555 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/pl/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/pt/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/pt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7748 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/pt/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      219 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/pt/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/ro/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ro/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      734 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ro/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/ru/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ru/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      353 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ru/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3958 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ru/test_lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      220 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ru/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5983 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ru/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/sa/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sa/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1297 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sa/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/sk/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1485 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sk/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      453 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sk/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/sl/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      993 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sl/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sl/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/sq/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sq/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1178 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sq/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      817 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sq/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.276712 spacy-4.0.0.dev1/spacy/tests/lang/sr/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      510 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sr/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4302 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/sr/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.280712 spacy-4.0.0.dev1/spacy/tests/lang/sv/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2453 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      683 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/test_lex_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1857 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      723 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1005 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/sv/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.280712 spacy-4.0.0.dev1/spacy/tests/lang/ta/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2737 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ta/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7829 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/ta/test_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3322 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/test_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      924 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/test_initialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1910 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/test_lemmatizers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.280712 spacy-4.0.0.dev1/spacy/tests/lang/th/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/th/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      706 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/th/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      318 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/th/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.284712 spacy-4.0.0.dev1/spacy/tests/lang/ti/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ti/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ti/test_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2120 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ti/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.284712 spacy-4.0.0.dev1/spacy/tests/lang/tl/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/tl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      257 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/tl/test_indices.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4420 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/tl/test_punct.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2479 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/tl/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.284712 spacy-4.0.0.dev1/spacy/tests/lang/tr/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/tr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      422 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/tr/test_noun_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19784 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/tr/test_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1796 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/tr/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19589 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/tr/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.284712 spacy-4.0.0.dev1/spacy/tests/lang/tt/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/tt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3721 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/tt/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.288712 spacy-4.0.0.dev1/spacy/tests/lang/uk/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/uk/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      837 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/uk/test_lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5416 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/uk/test_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      364 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/uk/test_tokenizer_exc.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.288712 spacy-4.0.0.dev1/spacy/tests/lang/ur/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ur/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      229 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ur/test_prefix_suffix_infix.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      479 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/ur/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.288712 spacy-4.0.0.dev1/spacy/tests/lang/vi/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/vi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/vi/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1677 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/vi/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.288712 spacy-4.0.0.dev1/spacy/tests/lang/yo/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/yo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1490 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/yo/test_text.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.288712 spacy-4.0.0.dev1/spacy/tests/lang/zh/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/zh/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1245 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/zh/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/lang/zh/test_text.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2819 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/lang/zh/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.292712 spacy-4.0.0.dev1/spacy/tests/matcher/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/matcher/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14870 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/matcher/test_dependency_matcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2797 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/matcher/test_levenshtein.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30055 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/matcher/test_matcher_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    27183 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/matcher/test_matcher_logic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3334 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/matcher/test_pattern_validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17364 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/matcher/test_phrase_matcher.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.292712 spacy-4.0.0.dev1/spacy/tests/morphology/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/morphology/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      856 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/morphology/test_morph_converters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1348 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/morphology/test_morph_features.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      668 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/morphology/test_morph_pickle.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.292712 spacy-4.0.0.dev1/spacy/tests/package/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/package/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy/tests/package/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)      857 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy/tests/package/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3613 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy/tests/package/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     3133 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/package/test_requirements.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.296712 spacy-4.0.0.dev1/spacy/tests/parser/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/parser/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3148 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/_search.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     4919 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_add_label.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10085 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_arc_eager_oracle.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30594 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2859 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_neural_parser.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3600 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_nn_beam.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6289 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_nonproj.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23905 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_parse.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_parse_navigate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2560 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_preset_sbd.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_search.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2927 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_space_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1894 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/parser/test_state.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.304712 spacy-4.0.0.dev1/spacy/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3456 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3338 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_annotates_on_update.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9535 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_attributeruler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12802 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_edit_tree_lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    47335 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_entity_linker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20789 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_entity_ruler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3188 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2350 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_initialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3725 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_lemmatizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3842 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9077 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_morphologizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19895 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_pipe_factories.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23092 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_pipe_methods.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18273 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_sentencizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4294 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_senter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7470 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_span_finder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16247 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_span_ruler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22723 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9803 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_tagger.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    37365 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21318 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/pipeline/test_tok2vec.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.304712 spacy-4.0.0.dev1/spacy/tests/serialize/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/serialize/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4183 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_resource_warning.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17271 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7370 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_doc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4028 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_docbin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      945 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_extension_attrs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7088 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_kb.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3594 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_language.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14977 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8766 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_span_groups.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7159 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_vocab_strings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      447 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    50002 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7765 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13600 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_displacy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/test_errors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31658 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_language.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13415 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_misc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9089 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_models.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2022 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_pickles.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17502 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_scorer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10600 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/test_symbols.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      748 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/test_ty.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.308712 spacy-4.0.0.dev1/spacy/tests/tokenizer/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2591 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/sun.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     1756 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4901 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/test_explain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7466 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/test_naughty_strings.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18589 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/test_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6605 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/test_urls.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1295 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/tokenizer/test_whitespace.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.312712 spacy-4.0.0.dev1/spacy/tests/training/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/training/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10607 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_augmenters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_corpus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_logger.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_loop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16145 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_new_example.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12027 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_pretraining.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3947 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_readers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6405 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_rehearse.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    46167 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/training/test_training.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3279 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.312712 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2821 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_lexeme.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4651 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_lookups.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3834 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_similarity.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3939 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_stringstore.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22339 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_vectors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2147 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_vocab_api.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokenizer.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    36344 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokenizer.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.320712 spacy-4.0.0.dev1/spacy/tokens/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tokens/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      248 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1667 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/doc.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5993 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/doc.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    83709 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/doc.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    12099 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/doc_bin.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      295 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/graph.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    23114 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/graph.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      303 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/morphanalysis.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/morphanalysis.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)     3073 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/morphanalysis.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      702 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/retokenizer.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    20434 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/retokenizer.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      632 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/span.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4175 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/span.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    37055 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/span.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      307 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/span_group.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      864 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/tokens/span_group.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    11804 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/span_group.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     4515 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/span_groups.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3419 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/token.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5346 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/token.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    32806 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/token.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     6926 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/tokens/underscore.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.324712 spacy-4.0.0.dev1/spacy/training/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/training/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)      897 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/align.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      614 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/alignment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      170 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/alignment_array.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     2128 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/alignment_array.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    13279 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/augment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9446 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/batchers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1269 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/callbacks.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.324712 spacy-4.0.0.dev1/spacy/training/converters/
+-rw-r--r--   0 vsts      (1001) docker     (122)      224 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/converters/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6179 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/converters/conll_ner_to_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10275 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/converters/conllu_to_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2356 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/converters/iob_to_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      884 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/converters/json_to_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11991 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/corpus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      327 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/example.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)    25036 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/example.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     8027 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/gold_io.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    17636 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/initialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9075 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/iob_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7819 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/loggers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26162 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/loop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9702 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/training/pretrain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1747 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      283 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/typedefs.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-23 12:17:53.000000 spacy-4.0.0.dev1/spacy/typedefs.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)    67017 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    25818 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/vectors.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     1199 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/vocab.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     2636 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/vocab.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)    22301 2023-06-23 12:17:54.000000 spacy-4.0.0.dev1/spacy/vocab.pyx
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-23 12:19:08.192711 spacy-4.0.0.dev1/spacy.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16877 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    29974 2023-06-23 12:19:08.000000 spacy-4.0.0.dev1/spacy.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       46 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)     1424 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-06-23 12:19:07.000000 spacy-4.0.0.dev1/spacy.egg-info/top_level.txt
```

### Comparing `spacy-4.0.0.dev0/LICENSE` & `spacy-4.0.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/PKG-INFO` & `spacy-4.0.0.dev1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy
-Version: 4.0.0.dev0
+Version: 4.0.0.dev1
 Summary: Industrial-strength Natural Language Processing (NLP) in Python
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spaCy/releases
 Project-URL: Source, https://github.com/explosion/spaCy
@@ -14,22 +14,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lookups
 Provides-Extra: transformers
 Provides-Extra: ray
 Provides-Extra: cuda
 Provides-Extra: cuda80
 Provides-Extra: cuda90
@@ -68,15 +66,18 @@
 state-of-the-art speed and **neural network models** for tagging,
 parsing, **named entity recognition**, **text classification** and more,
 multi-task learning with pretrained **transformers** like BERT, as well as a
 production-ready [**training system**](https://spacy.io/usage/training) and easy
 model packaging, deployment and workflow management. spaCy is commercial
 open-source software, released under the [MIT license](https://github.com/explosion/spaCy/blob/master/LICENSE).
 
-💫 **Version 3.4 out now!**
+💥 **We'd love to hear more about your experience with spaCy!**
+[Fill out our survey here.](https://form.typeform.com/to/aMel9q9f)
+
+💫 **Version 3.5 out now!**
 [Check out the release notes here.](https://github.com/explosion/spaCy/releases)
 
 [![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/8/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=8)
 [![Current Release Version](https://img.shields.io/github/release/explosion/spacy.svg?style=flat-square&logo=github)](https://github.com/explosion/spaCy/releases)
 [![pypi Version](https://img.shields.io/pypi/v/spacy.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy/)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/spacy.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/spacy)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
@@ -84,43 +85,44 @@
 <br />
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/spacy?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/spacy/)
 [![Conda downloads](https://img.shields.io/conda/dn/conda-forge/spacy?label=conda%20downloads)](https://anaconda.org/conda-forge/spacy)
 [![spaCy on Twitter](https://img.shields.io/twitter/follow/spacy_io.svg?style=social&label=Follow)](https://twitter.com/spacy_io)
 
 ## 📖 Documentation
 
-| Documentation                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                              |
-| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| ⭐️ **[spaCy 101]**                                                                                                                                                                                                       | New to spaCy? Here's everything you need to know!                                                                                                                                                                                                                                                                            |
-| 📚 **[Usage Guides]**                                                                                                                                                                                                     | How to use spaCy and its features.                                                                                                                                                                                                                                                                                           |
-| 🚀 **[New in v3.0]**                                                                                                                                                                                                      | New features, backwards incompatibilities and migration guide.                                                                                                                                                                                                                                                               |
-| 🪐 **[Project Templates]**                                                                                                                                                                                                | End-to-end workflows you can clone, modify and run.                                                                                                                                                                                                                                                                          |
-| 🎛 **[API Reference]**                                                                                                                                                                                                     | The detailed reference for spaCy's API.                                                                                                                                                                                                                                                                                      |
-| 📦 **[Models]**                                                                                                                                                                                                           | Download trained pipelines for spaCy.                                                                                                                                                                                                                                                                                        |
-| 🌌 **[Universe]**                                                                                                                                                                                                         | Plugins, extensions, demos and books from the spaCy ecosystem.                                                                                                                                                                                                                                                               |
-| 👩‍🏫 **[Online Course]**                                                                                                                                                                                                    | Learn spaCy in this free and interactive online course.                                                                                                                                                                                                                                                                      |
-| 📺 **[Videos]**                                                                                                                                                                                                           | Our YouTube channel with video tutorials, talks and more.                                                                                                                                                                                                                                                                    |
-| 🛠 **[Changelog]**                                                                                                                                                                                                         | Changes and version history.                                                                                                                                                                                                                                                                                                 |
-| 💝 **[Contribute]**                                                                                                                                                                                                       | How to contribute to the spaCy project and code base.                                                                                                                                                                                                                                                                        |
+| Documentation                 |                                                                        |
+| ----------------------------- | ---------------------------------------------------------------------- |
+| ⭐️ **[spaCy 101]**           | New to spaCy? Here's everything you need to know!                      |
+| 📚 **[Usage Guides]**         | How to use spaCy and its features.                                     |
+| 🚀 **[New in v3.0]**          | New features, backwards incompatibilities and migration guide.         |
+| 🪐 **[Project Templates]**    | End-to-end workflows you can clone, modify and run.                    |
+| 🎛 **[API Reference]**         | The detailed reference for spaCy's API.                                |
+| 📦 **[Models]**               | Download trained pipelines for spaCy.                                  |
+| 🌌 **[Universe]**             | Plugins, extensions, demos and books from the spaCy ecosystem.         |
+| ⚙️ **[spaCy VS Code Extension]** | Additional tooling and features for working with spaCy's config files. |
+| 👩‍🏫 **[Online Course]** | Learn spaCy in this free and interactive online course. |
+| 📺 **[Videos]** | Our YouTube channel with video tutorials, talks and more. |
+| 🛠 **[Changelog]** | Changes and version history. |
+| 💝 **[Contribute]** | How to contribute to the spaCy project and code base. |
 | <a href="https://explosion.ai/spacy-tailored-pipelines"><img src="https://user-images.githubusercontent.com/13643239/152853098-1c761611-ccb0-4ec6-9066-b234552831fe.png" width="125" alt="spaCy Tailored Pipelines"/></a> | Get a custom spaCy pipeline, tailor-made for your NLP problem by spaCy's core developers. Streamlined, production-ready, predictable and maintainable. Start by completing our 5-minute questionnaire to tell us what you need and we'll be in touch! **[Learn more &rarr;](https://explosion.ai/spacy-tailored-pipelines)** |
 | <a href="https://explosion.ai/spacy-tailored-analysis"><img src="https://user-images.githubusercontent.com/1019791/206151300-b00cd189-e503-4797-aa1e-1bb6344062c5.png" width="125" alt="spaCy Tailored Pipelines"/></a> | Bespoke advice for problem solving, strategy and analysis for applied NLP projects. Services include data strategy, code reviews, pipeline design and annotation coaching. Curious? Fill in our 5-minute questionnaire to tell us what you need and we'll be in touch! **[Learn more &rarr;](https://explosion.ai/spacy-tailored-analysis)** |
 
 [spacy 101]: https://spacy.io/usage/spacy-101
 [new in v3.0]: https://spacy.io/usage/v3
 [usage guides]: https://spacy.io/usage/
 [api reference]: https://spacy.io/api/
 [models]: https://spacy.io/models
 [universe]: https://spacy.io/universe
+[spaCy VS Code Extension]: https://github.com/explosion/spacy-vscode
 [videos]: https://www.youtube.com/c/ExplosionAI
 [online course]: https://course.spacy.io
 [project templates]: https://github.com/explosion/projects
 [changelog]: https://spacy.io/usage#changelog
 [contribute]: https://github.com/explosion/spaCy/blob/master/CONTRIBUTING.md
 
-
 ## 💬 Where to ask questions
 
 The spaCy project is maintained by the [spaCy team](https://explosion.ai/about).
 Please understand that we won't be able to provide individual support via email.
 We also believe that help is much more valuable if it's shared publicly, so that
 more people can benefit from it.
 
@@ -157,15 +159,15 @@
 ## ⏳ Install spaCy
 
 For detailed installation instructions, see the
 [documentation](https://spacy.io/usage).
 
 - **Operating system**: macOS / OS X · Linux · Windows (Cygwin, MinGW, Visual
   Studio)
-- **Python version**: Python 3.6+ (only 64 bit)
+- **Python version**: Python 3.8+ (only 64 bit)
 - **Package managers**: [pip] · [conda] (via `conda-forge`)
 
 [pip]: https://pypi.org/project/spacy/
 [conda]: https://anaconda.org/conda-forge/spacy
 
 ### pip
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: spacy Version: 4.0.0.dev0 Summary: Industrial-
+Metadata-Version: 2.1 Name: spacy Version: 4.0.0.dev1 Summary: Industrial-
 strength Natural Language Processing (NLP) in Python Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Project-URL: Release notes, https://github.com/explosion/spaCy/releases
 Project-URL: Source, https://github.com/explosion/spaCy Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Cython Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: lookups Provides-Extra:
-transformers Provides-Extra: ray Provides-Extra: cuda Provides-Extra: cuda80
-Provides-Extra: cuda90 Provides-Extra: cuda91 Provides-Extra: cuda92 Provides-
-Extra: cuda100 Provides-Extra: cuda101 Provides-Extra: cuda102 Provides-Extra:
-cuda110 Provides-Extra: cuda111 Provides-Extra: cuda112 Provides-Extra: cuda113
-Provides-Extra: cuda114 Provides-Extra: cuda115 Provides-Extra: cuda116
-Provides-Extra: cuda117 Provides-Extra: cuda11x Provides-Extra: cuda-autodetect
-Provides-Extra: apple Provides-Extra: ja Provides-Extra: ko Provides-Extra: th
-License-File: LICENSE [https://explosion.ai/assets/img/logo.svg] # spaCy:
-Industrial-strength NLP spaCy is a library for **advanced Natural Language
-Processing** in Python and Cython. It's built on the very latest research, and
-was designed from day one to be used in real products. spaCy comes with
-[pretrained pipelines](https://spacy.io/models) and currently supports
-tokenization and training for **70+ languages**. It features state-of-the-art
-speed and **neural network models** for tagging, parsing, **named entity
-recognition**, **text classification** and more, multi-task learning with
-pretrained **transformers** like BERT, as well as a production-ready
-[**training system**](https://spacy.io/usage/training) and easy model
-packaging, deployment and workflow management. spaCy is commercial open-source
-software, released under the [MIT license](https://github.com/explosion/spaCy/
-blob/master/LICENSE). ð« **Version 3.4 out now!** [Check out the release
-notes here.](https://github.com/explosion/spaCy/releases) [![Azure Pipelines]
-(https://img.shields.io/azure-devops/build/explosion-ai/public/8/
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: lookups Provides-Extra: transformers Provides-Extra:
+ray Provides-Extra: cuda Provides-Extra: cuda80 Provides-Extra: cuda90
+Provides-Extra: cuda91 Provides-Extra: cuda92 Provides-Extra: cuda100 Provides-
+Extra: cuda101 Provides-Extra: cuda102 Provides-Extra: cuda110 Provides-Extra:
+cuda111 Provides-Extra: cuda112 Provides-Extra: cuda113 Provides-Extra: cuda114
+Provides-Extra: cuda115 Provides-Extra: cuda116 Provides-Extra: cuda117
+Provides-Extra: cuda11x Provides-Extra: cuda-autodetect Provides-Extra: apple
+Provides-Extra: ja Provides-Extra: ko Provides-Extra: th License-File: LICENSE
+[https://explosion.ai/assets/img/logo.svg] # spaCy: Industrial-strength NLP
+spaCy is a library for **advanced Natural Language Processing** in Python and
+Cython. It's built on the very latest research, and was designed from day one
+to be used in real products. spaCy comes with [pretrained pipelines](https://
+spacy.io/models) and currently supports tokenization and training for **70+
+languages**. It features state-of-the-art speed and **neural network models**
+for tagging, parsing, **named entity recognition**, **text classification** and
+more, multi-task learning with pretrained **transformers** like BERT, as well
+as a production-ready [**training system**](https://spacy.io/usage/training)
+and easy model packaging, deployment and workflow management. spaCy is
+commercial open-source software, released under the [MIT license](https://
+github.com/explosion/spaCy/blob/master/LICENSE). ð¥ **We'd love to hear more
+about your experience with spaCy!** [Fill out our survey here.](https://
+form.typeform.com/to/aMel9q9f) ð« **Version 3.5 out now!** [Check out the
+release notes here.](https://github.com/explosion/spaCy/releases) [![Azure
+Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/8/
 master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://
 dev.azure.com/explosion-ai/public/_build?definitionId=8) [![Current Release
 Version](https://img.shields.io/github/release/explosion/spacy.svg?style=flat-
 square&logo=github)](https://github.com/explosion/spaCy/releases) [![pypi
 Version](https://img.shields.io/pypi/v/spacy.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy/) [![conda
 Version](https://img.shields.io/conda/vn/conda-forge/spacy.svg?style=flat-
@@ -52,76 +52,73 @@
 github.com/ambv/black)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/
 spacy?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)]
 (https://pypi.org/project/spacy/) [![Conda downloads](https://img.shields.io/
 conda/dn/conda-forge/spacy?label=conda%20downloads)](https://anaconda.org/
 conda-forge/spacy) [![spaCy on Twitter](https://img.shields.io/twitter/follow/
 spacy_io.svg?style=social&label=Follow)](https://twitter.com/spacy_io) ## ð
-Documentation | Documentation | | | -------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
----------------- | ------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-------------------- | | â­ï¸ **[spaCy 101]** | New to spaCy? Here's
-everything you need to know! | | ð **[Usage Guides]** | How to use spaCy and
-its features. | | ð **[New in v3.0]** | New features, backwards
-incompatibilities and migration guide. | | ðª **[Project Templates]** | End-
-to-end workflows you can clone, modify and run. | | ð **[API Reference]** |
-The detailed reference for spaCy's API. | | ð¦ **[Models]** | Download
-trained pipelines for spaCy. | | ð **[Universe]** | Plugins, extensions,
-demos and books from the spaCy ecosystem. | | ð©âð« **[Online Course]** |
-Learn spaCy in this free and interactive online course. | | ðº **[Videos]** |
-Our YouTube channel with video tutorials, talks and more. | | ð  **
-[Changelog]** | Changes and version history. | | ð **[Contribute]** | How to
-contribute to the spaCy project and code base. | | [spaCy_Tailored_Pipelines] |
-Get a custom spaCy pipeline, tailor-made for your NLP problem by spaCy's core
-developers. Streamlined, production-ready, predictable and maintainable. Start
-by completing our 5-minute questionnaire to tell us what you need and we'll be
-in touch! **[Learn more →](https://explosion.ai/spacy-tailored-pipelines)** | |
+Documentation | Documentation | | | ----------------------------- | -----------
+----------------------------------------------------------- | | â­ï¸ **[spaCy
+101]** | New to spaCy? Here's everything you need to know! | | ð **[Usage
+Guides]** | How to use spaCy and its features. | | ð **[New in v3.0]** | New
+features, backwards incompatibilities and migration guide. | | ðª **[Project
+Templates]** | End-to-end workflows you can clone, modify and run. | | ð **
+[API Reference]** | The detailed reference for spaCy's API. | | ð¦ **
+[Models]** | Download trained pipelines for spaCy. | | ð **[Universe]** |
+Plugins, extensions, demos and books from the spaCy ecosystem. | | âï¸ **
+[spaCy VS Code Extension]** | Additional tooling and features for working with
+spaCy's config files. | | ð©âð« **[Online Course]** | Learn spaCy in this
+free and interactive online course. | | ðº **[Videos]** | Our YouTube channel
+with video tutorials, talks and more. | | ð  **[Changelog]** | Changes and
+version history. | | ð **[Contribute]** | How to contribute to the spaCy
+project and code base. | | [spaCy_Tailored_Pipelines] | Get a custom spaCy
+pipeline, tailor-made for your NLP problem by spaCy's core developers.
+Streamlined, production-ready, predictable and maintainable. Start by
+completing our 5-minute questionnaire to tell us what you need and we'll be in
+touch! **[Learn more →](https://explosion.ai/spacy-tailored-pipelines)** | |
 [spaCy_Tailored_Pipelines] | Bespoke advice for problem solving, strategy and
 analysis for applied NLP projects. Services include data strategy, code
 reviews, pipeline design and annotation coaching. Curious? Fill in our 5-minute
 questionnaire to tell us what you need and we'll be in touch! **[Learn more →]
 (https://explosion.ai/spacy-tailored-analysis)** | [spacy 101]: https://
 spacy.io/usage/spacy-101 [new in v3.0]: https://spacy.io/usage/v3 [usage
 guides]: https://spacy.io/usage/ [api reference]: https://spacy.io/api/
-[models]: https://spacy.io/models [universe]: https://spacy.io/universe
-[videos]: https://www.youtube.com/c/ExplosionAI [online course]: https://
-course.spacy.io [project templates]: https://github.com/explosion/projects
-[changelog]: https://spacy.io/usage#changelog [contribute]: https://github.com/
-explosion/spaCy/blob/master/CONTRIBUTING.md ## ð¬ Where to ask questions The
-spaCy project is maintained by the [spaCy team](https://explosion.ai/about).
-Please understand that we won't be able to provide individual support via
-email. We also believe that help is much more valuable if it's shared publicly,
-so that more people can benefit from it. | Type | Platforms | | ---------------
----------------- | --------------------------------------- | | ð¨ **Bug
-Reports** | [GitHub Issue Tracker] | | ð **Feature Requests & Ideas** |
-[GitHub Discussions] | | ð©âð» **Usage Questions** | [GitHub Discussions]
-Â· [Stack Overflow] | | ð¯ **General Discussion** | [GitHub Discussions] |
-[github issue tracker]: https://github.com/explosion/spaCy/issues [github
-discussions]: https://github.com/explosion/spaCy/discussions [stack overflow]:
-https://stackoverflow.com/questions/tagged/spacy ## Features - Support for
-**70+ languages** - **Trained pipelines** for different languages and tasks -
-Multi-task learning with pretrained **transformers** like BERT - Support for
+[models]: https://spacy.io/models [universe]: https://spacy.io/universe [spaCy
+VS Code Extension]: https://github.com/explosion/spacy-vscode [videos]: https:/
+/www.youtube.com/c/ExplosionAI [online course]: https://course.spacy.io
+[project templates]: https://github.com/explosion/projects [changelog]: https:/
+/spacy.io/usage#changelog [contribute]: https://github.com/explosion/spaCy/
+blob/master/CONTRIBUTING.md ## ð¬ Where to ask questions The spaCy project is
+maintained by the [spaCy team](https://explosion.ai/about). Please understand
+that we won't be able to provide individual support via email. We also believe
+that help is much more valuable if it's shared publicly, so that more people
+can benefit from it. | Type | Platforms | | ------------------------------- | -
+-------------------------------------- | | ð¨ **Bug Reports** | [GitHub Issue
+Tracker] | | ð **Feature Requests & Ideas** | [GitHub Discussions] | |
+ð©âð» **Usage Questions** | [GitHub Discussions] Â· [Stack Overflow] | |
+ð¯ **General Discussion** | [GitHub Discussions] | [github issue tracker]:
+https://github.com/explosion/spaCy/issues [github discussions]: https://
+github.com/explosion/spaCy/discussions [stack overflow]: https://
+stackoverflow.com/questions/tagged/spacy ## Features - Support for **70+
+languages** - **Trained pipelines** for different languages and tasks - Multi-
+task learning with pretrained **transformers** like BERT - Support for
 pretrained **word vectors** and embeddings - State-of-the-art speed -
 Production-ready **training system** - Linguistically-motivated
 **tokenization** - Components for named **entity recognition**, part-of-speech-
 tagging, dependency parsing, sentence segmentation, **text classification**,
 lemmatization, morphological analysis, entity linking and more - Easily
 extensible with **custom components** and attributes - Support for custom
 models in **PyTorch**, **TensorFlow** and other frameworks - Built in
 **visualizers** for syntax and NER - Easy **model packaging**, deployment and
 workflow management - Robust, rigorously evaluated accuracy ð **For more
 details, see the [facts, figures and benchmarks](https://spacy.io/usage/facts-
 figures).** ## â³ Install spaCy For detailed installation instructions, see
 the [documentation](https://spacy.io/usage). - **Operating system**: macOS / OS
 X Â· Linux Â· Windows (Cygwin, MinGW, Visual Studio) - **Python version**:
-Python 3.6+ (only 64 bit) - **Package managers**: [pip] Â· [conda] (via `conda-
+Python 3.8+ (only 64 bit) - **Package managers**: [pip] Â· [conda] (via `conda-
 forge`) [pip]: https://pypi.org/project/spacy/ [conda]: https://anaconda.org/
 conda-forge/spacy ### pip Using pip, spaCy releases are available as source
 packages and binary wheels. Before you install spaCy and its dependencies, make
 sure that your `pip`, `setuptools` and `wheel` are up to date. ```bash pip
 install -U pip setuptools wheel pip install spacy ``` To install additional
 data tables for lemmatization and normalization you can run `pip install spacy
 [lookups]` or install [`spacy-lookups-data`](https://github.com/explosion/
```

### Comparing `spacy-4.0.0.dev0/README.md` & `spacy-4.0.0.dev1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 state-of-the-art speed and **neural network models** for tagging,
 parsing, **named entity recognition**, **text classification** and more,
 multi-task learning with pretrained **transformers** like BERT, as well as a
 production-ready [**training system**](https://spacy.io/usage/training) and easy
 model packaging, deployment and workflow management. spaCy is commercial
 open-source software, released under the [MIT license](https://github.com/explosion/spaCy/blob/master/LICENSE).
 
-💫 **Version 3.4 out now!**
+💥 **We'd love to hear more about your experience with spaCy!**
+[Fill out our survey here.](https://form.typeform.com/to/aMel9q9f)
+
+💫 **Version 3.5 out now!**
 [Check out the release notes here.](https://github.com/explosion/spaCy/releases)
 
 [![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/8/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=8)
 [![Current Release Version](https://img.shields.io/github/release/explosion/spacy.svg?style=flat-square&logo=github)](https://github.com/explosion/spaCy/releases)
 [![pypi Version](https://img.shields.io/pypi/v/spacy.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy/)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/spacy.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/spacy)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
@@ -28,43 +31,44 @@
 <br />
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/spacy?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/spacy/)
 [![Conda downloads](https://img.shields.io/conda/dn/conda-forge/spacy?label=conda%20downloads)](https://anaconda.org/conda-forge/spacy)
 [![spaCy on Twitter](https://img.shields.io/twitter/follow/spacy_io.svg?style=social&label=Follow)](https://twitter.com/spacy_io)
 
 ## 📖 Documentation
 
-| Documentation                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                              |
-| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| ⭐️ **[spaCy 101]**                                                                                                                                                                                                       | New to spaCy? Here's everything you need to know!                                                                                                                                                                                                                                                                            |
-| 📚 **[Usage Guides]**                                                                                                                                                                                                     | How to use spaCy and its features.                                                                                                                                                                                                                                                                                           |
-| 🚀 **[New in v3.0]**                                                                                                                                                                                                      | New features, backwards incompatibilities and migration guide.                                                                                                                                                                                                                                                               |
-| 🪐 **[Project Templates]**                                                                                                                                                                                                | End-to-end workflows you can clone, modify and run.                                                                                                                                                                                                                                                                          |
-| 🎛 **[API Reference]**                                                                                                                                                                                                     | The detailed reference for spaCy's API.                                                                                                                                                                                                                                                                                      |
-| 📦 **[Models]**                                                                                                                                                                                                           | Download trained pipelines for spaCy.                                                                                                                                                                                                                                                                                        |
-| 🌌 **[Universe]**                                                                                                                                                                                                         | Plugins, extensions, demos and books from the spaCy ecosystem.                                                                                                                                                                                                                                                               |
-| 👩‍🏫 **[Online Course]**                                                                                                                                                                                                    | Learn spaCy in this free and interactive online course.                                                                                                                                                                                                                                                                      |
-| 📺 **[Videos]**                                                                                                                                                                                                           | Our YouTube channel with video tutorials, talks and more.                                                                                                                                                                                                                                                                    |
-| 🛠 **[Changelog]**                                                                                                                                                                                                         | Changes and version history.                                                                                                                                                                                                                                                                                                 |
-| 💝 **[Contribute]**                                                                                                                                                                                                       | How to contribute to the spaCy project and code base.                                                                                                                                                                                                                                                                        |
+| Documentation                 |                                                                        |
+| ----------------------------- | ---------------------------------------------------------------------- |
+| ⭐️ **[spaCy 101]**           | New to spaCy? Here's everything you need to know!                      |
+| 📚 **[Usage Guides]**         | How to use spaCy and its features.                                     |
+| 🚀 **[New in v3.0]**          | New features, backwards incompatibilities and migration guide.         |
+| 🪐 **[Project Templates]**    | End-to-end workflows you can clone, modify and run.                    |
+| 🎛 **[API Reference]**         | The detailed reference for spaCy's API.                                |
+| 📦 **[Models]**               | Download trained pipelines for spaCy.                                  |
+| 🌌 **[Universe]**             | Plugins, extensions, demos and books from the spaCy ecosystem.         |
+| ⚙️ **[spaCy VS Code Extension]** | Additional tooling and features for working with spaCy's config files. |
+| 👩‍🏫 **[Online Course]** | Learn spaCy in this free and interactive online course. |
+| 📺 **[Videos]** | Our YouTube channel with video tutorials, talks and more. |
+| 🛠 **[Changelog]** | Changes and version history. |
+| 💝 **[Contribute]** | How to contribute to the spaCy project and code base. |
 | <a href="https://explosion.ai/spacy-tailored-pipelines"><img src="https://user-images.githubusercontent.com/13643239/152853098-1c761611-ccb0-4ec6-9066-b234552831fe.png" width="125" alt="spaCy Tailored Pipelines"/></a> | Get a custom spaCy pipeline, tailor-made for your NLP problem by spaCy's core developers. Streamlined, production-ready, predictable and maintainable. Start by completing our 5-minute questionnaire to tell us what you need and we'll be in touch! **[Learn more &rarr;](https://explosion.ai/spacy-tailored-pipelines)** |
 | <a href="https://explosion.ai/spacy-tailored-analysis"><img src="https://user-images.githubusercontent.com/1019791/206151300-b00cd189-e503-4797-aa1e-1bb6344062c5.png" width="125" alt="spaCy Tailored Pipelines"/></a> | Bespoke advice for problem solving, strategy and analysis for applied NLP projects. Services include data strategy, code reviews, pipeline design and annotation coaching. Curious? Fill in our 5-minute questionnaire to tell us what you need and we'll be in touch! **[Learn more &rarr;](https://explosion.ai/spacy-tailored-analysis)** |
 
 [spacy 101]: https://spacy.io/usage/spacy-101
 [new in v3.0]: https://spacy.io/usage/v3
 [usage guides]: https://spacy.io/usage/
 [api reference]: https://spacy.io/api/
 [models]: https://spacy.io/models
 [universe]: https://spacy.io/universe
+[spaCy VS Code Extension]: https://github.com/explosion/spacy-vscode
 [videos]: https://www.youtube.com/c/ExplosionAI
 [online course]: https://course.spacy.io
 [project templates]: https://github.com/explosion/projects
 [changelog]: https://spacy.io/usage#changelog
 [contribute]: https://github.com/explosion/spaCy/blob/master/CONTRIBUTING.md
 
-
 ## 💬 Where to ask questions
 
 The spaCy project is maintained by the [spaCy team](https://explosion.ai/about).
 Please understand that we won't be able to provide individual support via email.
 We also believe that help is much more valuable if it's shared publicly, so that
 more people can benefit from it.
 
@@ -101,15 +105,15 @@
 ## ⏳ Install spaCy
 
 For detailed installation instructions, see the
 [documentation](https://spacy.io/usage).
 
 - **Operating system**: macOS / OS X · Linux · Windows (Cygwin, MinGW, Visual
   Studio)
-- **Python version**: Python 3.6+ (only 64 bit)
+- **Python version**: Python 3.8+ (only 64 bit)
 - **Package managers**: [pip] · [conda] (via `conda-forge`)
 
 [pip]: https://pypi.org/project/spacy/
 [conda]: https://anaconda.org/conda-forge/spacy
 
 ### pip
```

#### html2text {}

```diff
@@ -5,98 +5,97 @@
 spacy.io/models) and currently supports tokenization and training for **70+
 languages**. It features state-of-the-art speed and **neural network models**
 for tagging, parsing, **named entity recognition**, **text classification** and
 more, multi-task learning with pretrained **transformers** like BERT, as well
 as a production-ready [**training system**](https://spacy.io/usage/training)
 and easy model packaging, deployment and workflow management. spaCy is
 commercial open-source software, released under the [MIT license](https://
-github.com/explosion/spaCy/blob/master/LICENSE). ð« **Version 3.4 out now!**
-[Check out the release notes here.](https://github.com/explosion/spaCy/
-releases) [![Azure Pipelines](https://img.shields.io/azure-devops/build/
-explosion-ai/public/8/master.svg?logo=azure-pipelines&style=flat-
-square&label=build)](https://dev.azure.com/explosion-ai/public/
-_build?definitionId=8) [![Current Release Version](https://img.shields.io/
-github/release/explosion/spacy.svg?style=flat-square&logo=github)](https://
-github.com/explosion/spaCy/releases) [![pypi Version](https://img.shields.io/
-pypi/v/spacy.svg?style=flat-square&logo=pypi&logoColor=white)](https://
-pypi.org/project/spacy/) [![conda Version](https://img.shields.io/conda/vn/
-conda-forge/spacy.svg?style=flat-square&logo=conda-forge&logoColor=white)]
-(https://anaconda.org/conda-forge/spacy) [![Python wheels](https://
-img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-
-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/
-releases) [![Code style: black](https://img.shields.io/badge/code%20style-
-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
+github.com/explosion/spaCy/blob/master/LICENSE). ð¥ **We'd love to hear more
+about your experience with spaCy!** [Fill out our survey here.](https://
+form.typeform.com/to/aMel9q9f) ð« **Version 3.5 out now!** [Check out the
+release notes here.](https://github.com/explosion/spaCy/releases) [![Azure
+Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/8/
+master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://
+dev.azure.com/explosion-ai/public/_build?definitionId=8) [![Current Release
+Version](https://img.shields.io/github/release/explosion/spacy.svg?style=flat-
+square&logo=github)](https://github.com/explosion/spaCy/releases) [![pypi
+Version](https://img.shields.io/pypi/v/spacy.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy/) [![conda
+Version](https://img.shields.io/conda/vn/conda-forge/spacy.svg?style=flat-
+square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/
+spacy) [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-
+4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://
+github.com/explosion/wheelwright/releases) [![Code style: black](https://
+img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://
+github.com/ambv/black)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/
 spacy?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)]
 (https://pypi.org/project/spacy/) [![Conda downloads](https://img.shields.io/
 conda/dn/conda-forge/spacy?label=conda%20downloads)](https://anaconda.org/
 conda-forge/spacy) [![spaCy on Twitter](https://img.shields.io/twitter/follow/
 spacy_io.svg?style=social&label=Follow)](https://twitter.com/spacy_io) ## ð
-Documentation | Documentation | | | -------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
----------------- | ------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-------------------- | | â­ï¸ **[spaCy 101]** | New to spaCy? Here's
-everything you need to know! | | ð **[Usage Guides]** | How to use spaCy and
-its features. | | ð **[New in v3.0]** | New features, backwards
-incompatibilities and migration guide. | | ðª **[Project Templates]** | End-
-to-end workflows you can clone, modify and run. | | ð **[API Reference]** |
-The detailed reference for spaCy's API. | | ð¦ **[Models]** | Download
-trained pipelines for spaCy. | | ð **[Universe]** | Plugins, extensions,
-demos and books from the spaCy ecosystem. | | ð©âð« **[Online Course]** |
-Learn spaCy in this free and interactive online course. | | ðº **[Videos]** |
-Our YouTube channel with video tutorials, talks and more. | | ð  **
-[Changelog]** | Changes and version history. | | ð **[Contribute]** | How to
-contribute to the spaCy project and code base. | | [spaCy_Tailored_Pipelines] |
-Get a custom spaCy pipeline, tailor-made for your NLP problem by spaCy's core
-developers. Streamlined, production-ready, predictable and maintainable. Start
-by completing our 5-minute questionnaire to tell us what you need and we'll be
-in touch! **[Learn more →](https://explosion.ai/spacy-tailored-pipelines)** | |
+Documentation | Documentation | | | ----------------------------- | -----------
+----------------------------------------------------------- | | â­ï¸ **[spaCy
+101]** | New to spaCy? Here's everything you need to know! | | ð **[Usage
+Guides]** | How to use spaCy and its features. | | ð **[New in v3.0]** | New
+features, backwards incompatibilities and migration guide. | | ðª **[Project
+Templates]** | End-to-end workflows you can clone, modify and run. | | ð **
+[API Reference]** | The detailed reference for spaCy's API. | | ð¦ **
+[Models]** | Download trained pipelines for spaCy. | | ð **[Universe]** |
+Plugins, extensions, demos and books from the spaCy ecosystem. | | âï¸ **
+[spaCy VS Code Extension]** | Additional tooling and features for working with
+spaCy's config files. | | ð©âð« **[Online Course]** | Learn spaCy in this
+free and interactive online course. | | ðº **[Videos]** | Our YouTube channel
+with video tutorials, talks and more. | | ð  **[Changelog]** | Changes and
+version history. | | ð **[Contribute]** | How to contribute to the spaCy
+project and code base. | | [spaCy_Tailored_Pipelines] | Get a custom spaCy
+pipeline, tailor-made for your NLP problem by spaCy's core developers.
+Streamlined, production-ready, predictable and maintainable. Start by
+completing our 5-minute questionnaire to tell us what you need and we'll be in
+touch! **[Learn more →](https://explosion.ai/spacy-tailored-pipelines)** | |
 [spaCy_Tailored_Pipelines] | Bespoke advice for problem solving, strategy and
 analysis for applied NLP projects. Services include data strategy, code
 reviews, pipeline design and annotation coaching. Curious? Fill in our 5-minute
 questionnaire to tell us what you need and we'll be in touch! **[Learn more →]
 (https://explosion.ai/spacy-tailored-analysis)** | [spacy 101]: https://
 spacy.io/usage/spacy-101 [new in v3.0]: https://spacy.io/usage/v3 [usage
 guides]: https://spacy.io/usage/ [api reference]: https://spacy.io/api/
-[models]: https://spacy.io/models [universe]: https://spacy.io/universe
-[videos]: https://www.youtube.com/c/ExplosionAI [online course]: https://
-course.spacy.io [project templates]: https://github.com/explosion/projects
-[changelog]: https://spacy.io/usage#changelog [contribute]: https://github.com/
-explosion/spaCy/blob/master/CONTRIBUTING.md ## ð¬ Where to ask questions The
-spaCy project is maintained by the [spaCy team](https://explosion.ai/about).
-Please understand that we won't be able to provide individual support via
-email. We also believe that help is much more valuable if it's shared publicly,
-so that more people can benefit from it. | Type | Platforms | | ---------------
----------------- | --------------------------------------- | | ð¨ **Bug
-Reports** | [GitHub Issue Tracker] | | ð **Feature Requests & Ideas** |
-[GitHub Discussions] | | ð©âð» **Usage Questions** | [GitHub Discussions]
-Â· [Stack Overflow] | | ð¯ **General Discussion** | [GitHub Discussions] |
-[github issue tracker]: https://github.com/explosion/spaCy/issues [github
-discussions]: https://github.com/explosion/spaCy/discussions [stack overflow]:
-https://stackoverflow.com/questions/tagged/spacy ## Features - Support for
-**70+ languages** - **Trained pipelines** for different languages and tasks -
-Multi-task learning with pretrained **transformers** like BERT - Support for
+[models]: https://spacy.io/models [universe]: https://spacy.io/universe [spaCy
+VS Code Extension]: https://github.com/explosion/spacy-vscode [videos]: https:/
+/www.youtube.com/c/ExplosionAI [online course]: https://course.spacy.io
+[project templates]: https://github.com/explosion/projects [changelog]: https:/
+/spacy.io/usage#changelog [contribute]: https://github.com/explosion/spaCy/
+blob/master/CONTRIBUTING.md ## ð¬ Where to ask questions The spaCy project is
+maintained by the [spaCy team](https://explosion.ai/about). Please understand
+that we won't be able to provide individual support via email. We also believe
+that help is much more valuable if it's shared publicly, so that more people
+can benefit from it. | Type | Platforms | | ------------------------------- | -
+-------------------------------------- | | ð¨ **Bug Reports** | [GitHub Issue
+Tracker] | | ð **Feature Requests & Ideas** | [GitHub Discussions] | |
+ð©âð» **Usage Questions** | [GitHub Discussions] Â· [Stack Overflow] | |
+ð¯ **General Discussion** | [GitHub Discussions] | [github issue tracker]:
+https://github.com/explosion/spaCy/issues [github discussions]: https://
+github.com/explosion/spaCy/discussions [stack overflow]: https://
+stackoverflow.com/questions/tagged/spacy ## Features - Support for **70+
+languages** - **Trained pipelines** for different languages and tasks - Multi-
+task learning with pretrained **transformers** like BERT - Support for
 pretrained **word vectors** and embeddings - State-of-the-art speed -
 Production-ready **training system** - Linguistically-motivated
 **tokenization** - Components for named **entity recognition**, part-of-speech-
 tagging, dependency parsing, sentence segmentation, **text classification**,
 lemmatization, morphological analysis, entity linking and more - Easily
 extensible with **custom components** and attributes - Support for custom
 models in **PyTorch**, **TensorFlow** and other frameworks - Built in
 **visualizers** for syntax and NER - Easy **model packaging**, deployment and
 workflow management - Robust, rigorously evaluated accuracy ð **For more
 details, see the [facts, figures and benchmarks](https://spacy.io/usage/facts-
 figures).** ## â³ Install spaCy For detailed installation instructions, see
 the [documentation](https://spacy.io/usage). - **Operating system**: macOS / OS
 X Â· Linux Â· Windows (Cygwin, MinGW, Visual Studio) - **Python version**:
-Python 3.6+ (only 64 bit) - **Package managers**: [pip] Â· [conda] (via `conda-
+Python 3.8+ (only 64 bit) - **Package managers**: [pip] Â· [conda] (via `conda-
 forge`) [pip]: https://pypi.org/project/spacy/ [conda]: https://anaconda.org/
 conda-forge/spacy ### pip Using pip, spaCy releases are available as source
 packages and binary wheels. Before you install spaCy and its dependencies, make
 sure that your `pip`, `setuptools` and `wheel` are up to date. ```bash pip
 install -U pip setuptools wheel pip install spacy ``` To install additional
 data tables for lemmatization and normalization you can run `pip install spacy
 [lookups]` or install [`spacy-lookups-data`](https://github.com/explosion/
```

### Comparing `spacy-4.0.0.dev0/licenses/3rd_party_licenses.txt` & `spacy-4.0.0.dev1/licenses/3rd_party_licenses.txt`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/setup.cfg` & `spacy-4.0.0.dev1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -13,99 +13,103 @@
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Cython
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 project_urls = 
 	Release notes = https://github.com/explosion/spaCy/releases
 	Source = https://github.com/explosion/spaCy
 
 [options]
 zip_safe = false
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
+setup_requires = 
+	cython>=0.25,<3.0
+	numpy>=1.15.0
+	cymem>=2.0.2,<2.1.0
+	preshed>=3.0.2,<3.1.0
+	murmurhash>=0.28.0,<1.1.0
+	thinc>=9.0.0.dev2,<9.1.0
 install_requires = 
-	spacy-legacy>=3.0.11,<3.1.0
+	spacy-legacy>=4.0.0.dev0,<4.1.0
 	spacy-loggers>=1.0.0,<2.0.0
 	murmurhash>=0.28.0,<1.1.0
 	cymem>=2.0.2,<2.1.0
 	preshed>=3.0.2,<3.1.0
 	thinc>=9.0.0.dev2,<9.1.0
 	wasabi>=0.9.1,<1.2.0
 	srsly>=2.4.3,<3.0.0
 	catalogue>=2.0.6,<2.1.0
-	typer>=0.3.0,<0.8.0
+	typer>=0.3.0,<0.10.0
 	pathy>=0.10.0
 	smart-open>=5.2.1,<7.0.0
 	tqdm>=4.38.0,<5.0.0
 	numpy>=1.15.0
 	requests>=2.13.0,<3.0.0
 	pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
 	jinja2
 	setuptools
 	packaging>=20.0
-	typing_extensions>=3.7.4,<4.2.0; python_version < "3.8"
 	langcodes>=3.2.0,<4.0.0
 
 [options.entry_points]
 console_scripts = 
 	spacy = spacy.cli:setup_cli
 
 [options.extras_require]
 lookups = 
 	spacy_lookups_data>=1.0.3,<1.1.0
 transformers = 
 	spacy_transformers>=1.1.2,<1.3.0
 ray = 
 	spacy_ray>=0.1.0,<1.0.0
 cuda = 
-	cupy>=5.0.0b4,<12.0.0
+	cupy>=5.0.0b4,<13.0.0
 cuda80 = 
-	cupy-cuda80>=5.0.0b4,<12.0.0
+	cupy-cuda80>=5.0.0b4,<13.0.0
 cuda90 = 
-	cupy-cuda90>=5.0.0b4,<12.0.0
+	cupy-cuda90>=5.0.0b4,<13.0.0
 cuda91 = 
-	cupy-cuda91>=5.0.0b4,<12.0.0
+	cupy-cuda91>=5.0.0b4,<13.0.0
 cuda92 = 
-	cupy-cuda92>=5.0.0b4,<12.0.0
+	cupy-cuda92>=5.0.0b4,<13.0.0
 cuda100 = 
-	cupy-cuda100>=5.0.0b4,<12.0.0
+	cupy-cuda100>=5.0.0b4,<13.0.0
 cuda101 = 
-	cupy-cuda101>=5.0.0b4,<12.0.0
+	cupy-cuda101>=5.0.0b4,<13.0.0
 cuda102 = 
-	cupy-cuda102>=5.0.0b4,<12.0.0
+	cupy-cuda102>=5.0.0b4,<13.0.0
 cuda110 = 
-	cupy-cuda110>=5.0.0b4,<12.0.0
+	cupy-cuda110>=5.0.0b4,<13.0.0
 cuda111 = 
-	cupy-cuda111>=5.0.0b4,<12.0.0
+	cupy-cuda111>=5.0.0b4,<13.0.0
 cuda112 = 
-	cupy-cuda112>=5.0.0b4,<12.0.0
+	cupy-cuda112>=5.0.0b4,<13.0.0
 cuda113 = 
-	cupy-cuda113>=5.0.0b4,<12.0.0
+	cupy-cuda113>=5.0.0b4,<13.0.0
 cuda114 = 
-	cupy-cuda114>=5.0.0b4,<12.0.0
+	cupy-cuda114>=5.0.0b4,<13.0.0
 cuda115 = 
-	cupy-cuda115>=5.0.0b4,<12.0.0
+	cupy-cuda115>=5.0.0b4,<13.0.0
 cuda116 = 
-	cupy-cuda116>=5.0.0b4,<12.0.0
+	cupy-cuda116>=5.0.0b4,<13.0.0
 cuda117 = 
-	cupy-cuda117>=5.0.0b4,<12.0.0
+	cupy-cuda117>=5.0.0b4,<13.0.0
 cuda11x = 
-	cupy-cuda11x>=11.0.0,<12.0.0
+	cupy-cuda11x>=11.0.0,<13.0.0
 cuda-autodetect = 
-	cupy-wheel>=11.0.0,<12.0.0
+	cupy-wheel>=11.0.0,<13.0.0
 apple = 
 	thinc-apple-ops>=0.1.0.dev0,<1.0.0
 ja = 
 	sudachipy>=0.5.2,!=0.6.1
 	sudachidict_core>=20211220
 ko = 
 	mecab-ko>=1.0.0
```

### Comparing `spacy-4.0.0.dev0/setup.py` & `spacy-4.0.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/__init__.py` & `spacy-4.0.0.dev1/spacy/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/attrs.pxd` & `spacy-4.0.0.dev1/spacy/attrs.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/attrs.pyx` & `spacy-4.0.0.dev1/spacy/attrs.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/__init__.py` & `spacy-4.0.0.dev1/spacy/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from wasabi import msg
 
 from ._util import app, setup_cli  # noqa: F401
 
 # These are the actual functions, NOT the wrapped CLI commands. The CLI commands
 # are registered automatically and won't have to be imported here.
+from .benchmark_speed import benchmark_speed_cli  # noqa: F401
 from .download import download  # noqa: F401
 from .info import info  # noqa: F401
 from .package import package  # noqa: F401
 from .profile import profile  # noqa: F401
 from .train import train_cli  # noqa: F401
 from .assemble import assemble_cli  # noqa: F401
 from .pretrain import pretrain  # noqa: F401
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/_util.py` & `spacy-4.0.0.dev1/spacy/cli/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any, Union, List, Optional, Tuple, Iterable
+from typing import Dict, Any, Union, List, Optional, Tuple, Iterable, Literal
 from typing import TYPE_CHECKING, overload
 import sys
 import shutil
 from pathlib import Path
 from wasabi import msg, Printer
 import srsly
 import hashlib
@@ -12,18 +12,18 @@
 from typer.main import get_command
 from contextlib import contextmanager
 from thinc.api import Config, ConfigValidationError, require_gpu
 from thinc.util import gpu_is_available
 from configparser import InterpolationError
 import os
 
-from ..compat import Literal
 from ..schemas import ProjectConfigSchema, validate
 from ..util import import_file, run_command, make_tempdir, registry, logger
 from ..util import is_compatible_version, SimpleFrozenDict, ENV_VARS
+from ..errors import RENAMED_LANGUAGE_CODES
 from .. import about
 
 if TYPE_CHECKING:
     from pathy import FluidPath  # noqa: F401
 
 
 SDIST_SUFFIX = ".tar.gz"
@@ -42,28 +42,31 @@
 fetching its assets like datasets etc. See the project's {PROJECT_FILE} for the
 available commands.
 """
 DEBUG_HELP = """Suite of helpful commands for debugging and profiling. Includes
 commands to check and validate your config files, training and evaluation data,
 and custom model implementations.
 """
+BENCHMARK_HELP = """Commands for benchmarking pipelines."""
 INIT_HELP = """Commands for initializing configs and pipeline packages."""
 
 # Wrappers for Typer's annotations. Initially created to set defaults and to
 # keep the names short, but not needed at the moment.
 Arg = typer.Argument
 Opt = typer.Option
 
 app = typer.Typer(name=NAME, help=HELP)
+benchmark_cli = typer.Typer(name="benchmark", help=BENCHMARK_HELP, no_args_is_help=True)
 project_cli = typer.Typer(name="project", help=PROJECT_HELP, no_args_is_help=True)
 debug_cli = typer.Typer(name="debug", help=DEBUG_HELP, no_args_is_help=True)
 init_cli = typer.Typer(name="init", help=INIT_HELP, no_args_is_help=True)
 
 app.add_typer(project_cli)
 app.add_typer(debug_cli)
+app.add_typer(benchmark_cli)
 app.add_typer(init_cli)
 
 
 def setup_cli() -> None:
     # Make sure the entry-point for CLI runs, so that they get imported.
     registry.cli.get_all()
     # Ensure that the help messages always display the correct prompt
@@ -83,17 +86,17 @@
     RETURNS (Dict[str, Any]): The parsed dict, keyed by nested config setting.
     """
     env_string = os.environ.get(env_var, "") if env_var else ""
     env_overrides = _parse_overrides(split_arg_string(env_string))
     cli_overrides = _parse_overrides(args, is_cli=True)
     if cli_overrides:
         keys = [k for k in cli_overrides if k not in env_overrides]
-        logger.debug(f"Config overrides from CLI: {keys}")
+        logger.debug("Config overrides from CLI: %s", keys)
     if env_overrides:
-        logger.debug(f"Config overrides from env variables: {list(env_overrides)}")
+        logger.debug("Config overrides from env variables: %s", list(env_overrides))
     return {**cli_overrides, **env_overrides}
 
 
 def _parse_overrides(args: List[str], is_cli: bool = False) -> Dict[str, Any]:
     result = {}
     while args:
         opt = args.pop(0)
@@ -128,14 +131,24 @@
     # TODO: improve logic to handle simple types like list of strings?
     try:
         return srsly.json_loads(value)
     except ValueError:
         return str(value)
 
 
+def _handle_renamed_language_codes(lang: Optional[str]) -> None:
+    # Throw error for renamed language codes in v4
+    if lang in RENAMED_LANGUAGE_CODES:
+        msg.fail(
+            title="Renamed language code",
+            text=f"Language code '{lang}' was replaced with '{RENAMED_LANGUAGE_CODES[lang]}' in spaCy v4. Update the language code from '{lang}' to '{RENAMED_LANGUAGE_CODES[lang]}'.",
+            exits=1,
+        )
+
+
 def load_project_config(
     path: Path, interpolate: bool = True, overrides: Dict[str, Any] = SimpleFrozenDict()
 ) -> Dict[str, Any]:
     """Load the project.yml file from a directory and validate it. Also make
     sure that all directories defined in the config exist.
 
     path (Path): The path to the project directory.
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/apply.py` & `spacy-4.0.0.dev1/spacy/cli/apply.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/assemble.py` & `spacy-4.0.0.dev1/spacy/cli/assemble.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/convert.py` & `spacy-4.0.0.dev1/spacy/cli/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from wasabi import Printer
 import srsly
 import re
 import sys
 import itertools
 
-from ._util import app, Arg, Opt, walk_directory
+from ._util import app, Arg, Opt, _handle_renamed_language_codes, walk_directory
 from ..training import docs_to_json
 from ..tokens import Doc, DocBin
 from ..training.converters import iob_to_docs, conll_ner_to_docs, json_to_docs
 from ..training.converters import conllu_to_docs
 
 
 # Converters are matched by file extension except for ner/iob, which are
@@ -108,14 +108,18 @@
     concatenate: bool = False,
     silent: bool = True,
     msg: Optional[Printer] = None,
 ) -> None:
     input_path = Path(input_path)
     if not msg:
         msg = Printer(no_print=silent)
+
+    # Throw error for renamed language codes in v4
+    _handle_renamed_language_codes(lang)
+
     ner_map = srsly.read_json(ner_map) if ner_map is not None else None
     doc_files = []
     for input_loc in walk_directory(input_path, converter):
         with input_loc.open("r", encoding="utf-8") as infile:
             input_data = infile.read()
         # Use converter function to convert data
         func = CONVERTERS[converter]
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/debug_config.py` & `spacy-4.0.0.dev1/spacy/cli/debug_config.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/debug_data.py` & `spacy-4.0.0.dev1/spacy/cli/debug_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Tuple, Union
-from typing import cast, overload
+from typing import Literal, cast, overload
 from pathlib import Path
 from collections import Counter
 import sys
 import srsly
 from wasabi import Printer, MESSAGES, msg
 import typer
 import math
+import numpy
 
 from ._util import app, Arg, Opt, show_validation_error, parse_config_overrides
 from ._util import import_code, debug_cli, _format_number
 from ..training import Example, remove_bilu_prefix
 from ..training.initialize import get_sourced_components
 from ..schemas import ConfigSchemaTraining
 from ..pipeline import TrainablePipe
 from ..pipeline._parser_internals import nonproj
 from ..pipeline._parser_internals.nonproj import DELIMITER
 from ..pipeline import Morphologizer, SpanCategorizer
+from ..pipeline._edit_tree_internals.edit_trees import EditTrees
 from ..morphology import Morphology
 from ..language import Language
 from ..util import registry, resolve_dot_names
-from ..compat import Literal
 from ..vectors import Mode as VectorsMode
 from .. import util
 
 
 # Minimum number of expected occurrences of NER label in data to train new label
 NEW_LABEL_THRESHOLD = 50
 # Minimum number of expected occurrences of dependency labels
@@ -331,15 +332,15 @@
             msg.text(
                 "Training data should always include examples of spans "
                 "in context, as well as examples without a given span "
                 "type.",
                 show=verbose,
             )
         else:
-            msg.good("Examples without ocurrences available for all labels")
+            msg.good("Examples without occurrences available for all labels")
 
     if "ner" in factory_names:
         # Get all unique NER labels present in the data
         labels = set(
             label for label in gold_train_data["ner"] if label not in ("O", "-", None)
         )
         label_counts = gold_train_data["ner"]
@@ -516,17 +517,21 @@
                     "Train/dev mismatch: the dev data contains instances "
                     "without mutually-exclusive classes while the train data "
                     "contains only instances with mutually-exclusive classes."
                 )
 
     if "tagger" in factory_names:
         msg.divider("Part-of-speech Tagging")
-        label_list = [label for label in gold_train_data["tags"]]
-        model_labels = _get_labels_from_model(nlp, "tagger")
+        label_list, counts = zip(*gold_train_data["tags"].items())
         msg.info(f"{len(label_list)} label(s) in train data")
+        p = numpy.array(counts)
+        p = p / p.sum()
+        norm_entropy = (-p * numpy.log2(p)).sum() / numpy.log2(len(label_list))
+        msg.info(f"{norm_entropy} is the normalised label entropy")
+        model_labels = _get_labels_from_model(nlp, "tagger")
         labels = set(label_list)
         missing_labels = model_labels - labels
         if missing_labels:
             msg.warn(
                 "Some model labels are not present in the train data. The "
                 "model performance may be degraded for these labels after "
                 f"training: {_format_labels(missing_labels)}."
@@ -667,14 +672,67 @@
                 f"projectivized train sentence(s)"
             )
         if gold_train_data["n_cycles"] > 0:
             msg.fail(
                 f"Found {gold_train_data['n_cycles']} projectivized train sentence(s) with cycles"
             )
 
+    if "trainable_lemmatizer" in factory_names:
+        msg.divider("Trainable Lemmatizer")
+        trees_train: Set[str] = gold_train_data["lemmatizer_trees"]
+        trees_dev: Set[str] = gold_dev_data["lemmatizer_trees"]
+        # This is necessary context when someone is attempting to interpret whether the
+        # number of trees exclusively in the dev set is meaningful.
+        msg.info(f"{len(trees_train)} lemmatizer trees generated from training data")
+        msg.info(f"{len(trees_dev)} lemmatizer trees generated from dev data")
+        dev_not_train = trees_dev - trees_train
+
+        if len(dev_not_train) != 0:
+            pct = len(dev_not_train) / len(trees_dev)
+            msg.info(
+                f"{len(dev_not_train)} lemmatizer trees ({pct*100:.1f}% of dev trees)"
+                " were found exclusively in the dev data."
+            )
+        else:
+            # Would we ever expect this case? It seems like it would be pretty rare,
+            # and we might actually want a warning?
+            msg.info("All trees in dev data present in training data.")
+
+        if gold_train_data["n_low_cardinality_lemmas"] > 0:
+            n = gold_train_data["n_low_cardinality_lemmas"]
+            msg.warn(f"{n} training docs with 0 or 1 unique lemmas.")
+
+        if gold_dev_data["n_low_cardinality_lemmas"] > 0:
+            n = gold_dev_data["n_low_cardinality_lemmas"]
+            msg.warn(f"{n} dev docs with 0 or 1 unique lemmas.")
+
+        if gold_train_data["no_lemma_annotations"] > 0:
+            n = gold_train_data["no_lemma_annotations"]
+            msg.warn(f"{n} training docs with no lemma annotations.")
+        else:
+            msg.good("All training docs have lemma annotations.")
+
+        if gold_dev_data["no_lemma_annotations"] > 0:
+            n = gold_dev_data["no_lemma_annotations"]
+            msg.warn(f"{n} dev docs with no lemma annotations.")
+        else:
+            msg.good("All dev docs have lemma annotations.")
+
+        if gold_train_data["partial_lemma_annotations"] > 0:
+            n = gold_train_data["partial_lemma_annotations"]
+            msg.info(f"{n} training docs with partial lemma annotations.")
+        else:
+            msg.good("All training docs have complete lemma annotations.")
+
+        if gold_dev_data["partial_lemma_annotations"] > 0:
+            n = gold_dev_data["partial_lemma_annotations"]
+            msg.info(f"{n} dev docs with partial lemma annotations.")
+        else:
+            msg.good("All dev docs have complete lemma annotations.")
+
     msg.divider("Summary")
     good_counts = msg.counts[MESSAGES.GOOD]
     warn_counts = msg.counts[MESSAGES.WARN]
     fail_counts = msg.counts[MESSAGES.FAIL]
     if good_counts:
         msg.good(f"{good_counts} {'check' if good_counts == 1 else 'checks'} passed")
     if warn_counts:
@@ -728,15 +786,21 @@
         "words_missing_vectors": Counter(),
         "n_sents": 0,
         "n_nonproj": 0,
         "n_cycles": 0,
         "n_cats_multilabel": 0,
         "n_cats_bad_values": 0,
         "texts": set(),
+        "lemmatizer_trees": set(),
+        "no_lemma_annotations": 0,
+        "partial_lemma_annotations": 0,
+        "n_low_cardinality_lemmas": 0,
     }
+    if "trainable_lemmatizer" in factory_names:
+        trees = EditTrees(nlp.vocab.strings)
     for eg in examples:
         gold = eg.reference
         doc = eg.predicted
         valid_words = [x.text for x in gold]
         data["words"].update(valid_words)
         data["n_words"] += len(valid_words)
         align = eg.alignment
@@ -858,14 +922,33 @@
                 if head == i:
                     data["roots"].update([dep])
                     data["n_sents"] += 1
             if nonproj.is_nonproj_tree(aligned_heads):
                 data["n_nonproj"] += 1
             if nonproj.contains_cycle(aligned_heads):
                 data["n_cycles"] += 1
+        if "trainable_lemmatizer" in factory_names:
+            # from EditTreeLemmatizer._labels_from_data
+            if all(token.lemma == 0 for token in gold):
+                data["no_lemma_annotations"] += 1
+                continue
+            if any(token.lemma == 0 for token in gold):
+                data["partial_lemma_annotations"] += 1
+            lemma_set = set()
+            for token in gold:
+                if token.lemma != 0:
+                    lemma_set.add(token.lemma)
+                    tree_id = trees.add(token.text, token.lemma_)
+                    tree_str = trees.tree_to_str(tree_id)
+                    data["lemmatizer_trees"].add(tree_str)
+            # We want to identify cases where lemmas aren't assigned
+            # or are all assigned the same value, as this would indicate
+            # an issue since we're expecting a large set of lemmas
+            if len(lemma_set) < 2 and len(gold) > 1:
+                data["n_low_cardinality_lemmas"] += 1
     return data
 
 
 @overload
 def _format_labels(labels: Iterable[str], counts: Literal[False] = False) -> str:
     ...
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/debug_diff.py` & `spacy-4.0.0.dev1/spacy/cli/debug_diff.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/debug_model.py` & `spacy-4.0.0.dev1/spacy/cli/debug_model.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/download.py` & `spacy-4.0.0.dev1/spacy/cli/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import sys
 from wasabi import msg
 import typer
 
 from ._util import app, Arg, Opt, WHEEL_SUFFIX, SDIST_SUFFIX
 from .. import about
 from ..util import is_package, get_minor_version, run_command
-from ..util import is_prerelease_version
+from ..util import is_prerelease_version, get_installed_models
+from ..util import get_package_version
 
 
 @app.command(
     "download",
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
 )
 def download_cli(
@@ -59,30 +60,35 @@
         model_name = "".join(components[:-1])
         version = components[-1]
     else:
         model_name = model
         compatibility = get_compatibility()
         version = get_version(model_name, compatibility)
 
+    # If we already have this version installed, skip downloading
+    installed = get_installed_models()
+    if model_name in installed:
+        installed_version = get_package_version(model_name)
+        if installed_version == version:
+            msg.warn(f"{model_name} v{version} already installed, skipping")
+            return
+
     filename = get_model_filename(model_name, version, sdist)
 
     download_model(filename, pip_args)
     msg.good(
         "Download and installation successful",
         f"You can now load the package via spacy.load('{model_name}')",
     )
 
 
 def get_model_filename(model_name: str, version: str, sdist: bool = False) -> str:
     dl_tpl = "{m}-{v}/{m}-{v}{s}"
-    egg_tpl = "#egg={m}=={v}"
     suffix = SDIST_SUFFIX if sdist else WHEEL_SUFFIX
     filename = dl_tpl.format(m=model_name, v=version, s=suffix)
-    if sdist:
-        filename += egg_tpl.format(m=model_name, v=version)
     return filename
 
 
 def get_compatibility() -> dict:
     if is_prerelease_version(about.__version__):
         version: Optional[str] = about.__version__
     else:
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/evaluate.py` & `spacy-4.0.0.dev1/spacy/cli/evaluate.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,133 +3,151 @@
 from pathlib import Path
 import re
 import srsly
 from thinc.api import fix_random_seed
 
 from ..training import Corpus
 from ..tokens import Doc
-from ._util import app, Arg, Opt, setup_gpu, import_code
+from ._util import app, Arg, Opt, setup_gpu, import_code, benchmark_cli
 from ..scorer import Scorer
 from .. import util
 from .. import displacy
 
 
+@benchmark_cli.command(
+    "accuracy",
+)
 @app.command("evaluate")
 def evaluate_cli(
     # fmt: off
     model: str = Arg(..., help="Model name or path"),
     data_path: Path = Arg(..., help="Location of binary evaluation data in .spacy format", exists=True),
     output: Optional[Path] = Opt(None, "--output", "-o", help="Output JSON file for metrics", dir_okay=False),
     code_path: Optional[Path] = Opt(None, "--code", "-c", help="Path to Python file with additional code (registered functions) to be imported"),
     use_gpu: int = Opt(-1, "--gpu-id", "-g", help="GPU ID or -1 for CPU"),
     gold_preproc: bool = Opt(False, "--gold-preproc", "-G", help="Use gold preprocessing"),
     displacy_path: Optional[Path] = Opt(None, "--displacy-path", "-dp", help="Directory to output rendered parses as HTML", exists=True, file_okay=False),
     displacy_limit: int = Opt(25, "--displacy-limit", "-dl", help="Limit of parses to render as HTML"),
+    per_component: bool = Opt(False, "--per-component", "-P", help="Return scores per component, only applicable when an output JSON file is specified."),
     # fmt: on
 ):
     """
     Evaluate a trained pipeline. Expects a loadable spaCy pipeline and evaluation
     data in the binary .spacy format. The --gold-preproc option sets up the
     evaluation examples with gold-standard sentences and tokens for the
     predictions. Gold preprocessing helps the annotations align to the
     tokenization, and may result in sequences of more consistent length. However,
     it may reduce runtime accuracy due to train/test skew. To render a sample of
     dependency parses in a HTML file, set as output directory as the
     displacy_path argument.
 
-    DOCS: https://spacy.io/api/cli#evaluate
+    DOCS: https://spacy.io/api/cli#benchmark-accuracy
     """
     import_code(code_path)
     evaluate(
         model,
         data_path,
         output=output,
         use_gpu=use_gpu,
         gold_preproc=gold_preproc,
         displacy_path=displacy_path,
         displacy_limit=displacy_limit,
+        per_component=per_component,
         silent=False,
     )
 
 
 def evaluate(
     model: str,
     data_path: Path,
     output: Optional[Path] = None,
     use_gpu: int = -1,
     gold_preproc: bool = False,
     displacy_path: Optional[Path] = None,
     displacy_limit: int = 25,
     silent: bool = True,
     spans_key: str = "sc",
+    per_component: bool = False,
 ) -> Dict[str, Any]:
     msg = Printer(no_print=silent, pretty=not silent)
     fix_random_seed()
     setup_gpu(use_gpu, silent=silent)
     data_path = util.ensure_path(data_path)
     output_path = util.ensure_path(output)
     displacy_path = util.ensure_path(displacy_path)
     if not data_path.exists():
         msg.fail("Evaluation data not found", data_path, exits=1)
     if displacy_path and not displacy_path.exists():
         msg.fail("Visualization output directory not found", displacy_path, exits=1)
     corpus = Corpus(data_path, gold_preproc=gold_preproc)
     nlp = util.load_model(model)
     dev_dataset = list(corpus(nlp))
-    scores = nlp.evaluate(dev_dataset)
-    metrics = {
-        "TOK": "token_acc",
-        "TAG": "tag_acc",
-        "POS": "pos_acc",
-        "MORPH": "morph_acc",
-        "LEMMA": "lemma_acc",
-        "UAS": "dep_uas",
-        "LAS": "dep_las",
-        "NER P": "ents_p",
-        "NER R": "ents_r",
-        "NER F": "ents_f",
-        "TEXTCAT": "cats_score",
-        "SENT P": "sents_p",
-        "SENT R": "sents_r",
-        "SENT F": "sents_f",
-        "SPAN P": f"spans_{spans_key}_p",
-        "SPAN R": f"spans_{spans_key}_r",
-        "SPAN F": f"spans_{spans_key}_f",
-        "SPEED": "speed",
-    }
-    results = {}
-    data = {}
-    for metric, key in metrics.items():
-        if key in scores:
-            if key == "cats_score":
-                metric = metric + " (" + scores.get("cats_score_desc", "unk") + ")"
-            if isinstance(scores[key], (int, float)):
-                if key == "speed":
-                    results[metric] = f"{scores[key]:.0f}"
+    scores = nlp.evaluate(dev_dataset, per_component=per_component)
+    if per_component:
+        data = scores
+        if output is None:
+            msg.warn(
+                "The per-component option is enabled but there is no output JSON file provided to save the scores to."
+            )
+        else:
+            msg.info("Per-component scores will be saved to output JSON file.")
+    else:
+        metrics = {
+            "TOK": "token_acc",
+            "TAG": "tag_acc",
+            "POS": "pos_acc",
+            "MORPH": "morph_acc",
+            "LEMMA": "lemma_acc",
+            "UAS": "dep_uas",
+            "LAS": "dep_las",
+            "NER P": "ents_p",
+            "NER R": "ents_r",
+            "NER F": "ents_f",
+            "TEXTCAT": "cats_score",
+            "SENT P": "sents_p",
+            "SENT R": "sents_r",
+            "SENT F": "sents_f",
+            "SPAN P": f"spans_{spans_key}_p",
+            "SPAN R": f"spans_{spans_key}_r",
+            "SPAN F": f"spans_{spans_key}_f",
+            "SPEED": "speed",
+        }
+        results = {}
+        data = {}
+        for metric, key in metrics.items():
+            if key in scores:
+                if key == "cats_score":
+                    metric = metric + " (" + scores.get("cats_score_desc", "unk") + ")"
+                if isinstance(scores[key], (int, float)):
+                    if key == "speed":
+                        results[metric] = f"{scores[key]:.0f}"
+                    else:
+                        results[metric] = f"{scores[key]*100:.2f}"
                 else:
-                    results[metric] = f"{scores[key]*100:.2f}"
-            else:
-                results[metric] = "-"
-            data[re.sub(r"[\s/]", "_", key.lower())] = scores[key]
+                    results[metric] = "-"
+                data[re.sub(r"[\s/]", "_", key.lower())] = scores[key]
 
-    msg.table(results, title="Results")
-    data = handle_scores_per_type(scores, data, spans_key=spans_key, silent=silent)
+        msg.table(results, title="Results")
+        data = handle_scores_per_type(scores, data, spans_key=spans_key, silent=silent)
 
     if displacy_path:
         factory_names = [nlp.get_pipe_meta(pipe).factory for pipe in nlp.pipe_names]
         docs = list(nlp.pipe(ex.reference.text for ex in dev_dataset[:displacy_limit]))
         render_deps = "parser" in factory_names
         render_ents = "ner" in factory_names
+        render_spans = "spancat" in factory_names
+
         render_parses(
             docs,
             displacy_path,
             model_name=model,
             limit=displacy_limit,
             deps=render_deps,
             ents=render_ents,
+            spans=render_spans,
         )
         msg.good(f"Generated {displacy_limit} parses as HTML", displacy_path)
 
     if output_path is not None:
         srsly.write_json(output_path, data)
         msg.good(f"Saved results to {output_path}")
     return data
@@ -175,27 +193,33 @@
 def render_parses(
     docs: List[Doc],
     output_path: Path,
     model_name: str = "",
     limit: int = 250,
     deps: bool = True,
     ents: bool = True,
+    spans: bool = True,
 ):
     docs[0].user_data["title"] = model_name
     if ents:
         html = displacy.render(docs[:limit], style="ent", page=True)
         with (output_path / "entities.html").open("w", encoding="utf8") as file_:
             file_.write(html)
     if deps:
         html = displacy.render(
             docs[:limit], style="dep", page=True, options={"compact": True}
         )
         with (output_path / "parses.html").open("w", encoding="utf8") as file_:
             file_.write(html)
 
+    if spans:
+        html = displacy.render(docs[:limit], style="span", page=True)
+        with (output_path / "spans.html").open("w", encoding="utf8") as file_:
+            file_.write(html)
+
 
 def print_prf_per_type(
     msg: Printer, scores: Dict[str, Dict[str, float]], name: str, type: str
 ) -> None:
     data = []
     for key, value in scores.items():
         row = [key]
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/find_threshold.py` & `spacy-4.0.0.dev1/spacy/cli/find_threshold.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     pipe_name: str = Arg(..., help="Name of pipe to examine thresholds for"),
     threshold_key: str = Arg(..., help="Key of threshold attribute in component's configuration"),
     scores_key: str = Arg(..., help="Metric to optimize"),
     n_trials: int = Opt(_DEFAULTS["n_trials"], "--n_trials", "-n", help="Number of trials to determine optimal thresholds"),
     code_path: Optional[Path] = Opt(None, "--code", "-c", help="Path to Python file with additional code (registered functions) to be imported"),
     use_gpu: int = Opt(_DEFAULTS["use_gpu"], "--gpu-id", "-g", help="GPU ID or -1 for CPU"),
     gold_preproc: bool = Opt(_DEFAULTS["gold_preproc"], "--gold-preproc", "-G", help="Use gold preprocessing"),
-    verbose: bool = Opt(False, "--silent", "-V", "-VV", help="Display more information for debugging purposes"),
+    verbose: bool = Opt(False, "--verbose", "-V", "-VV", help="Display more information for debugging purposes"),
     # fmt: on
 ):
     """
     Runs prediction trials for a trained model with varying tresholds to maximize
     the specified metric. The search space for the threshold is traversed linearly
     from 0 to 1 in `n_trials` steps. Results are displayed in a table on `stdout`
     (the corresponding API call to `spacy.cli.find_threshold.find_threshold()`
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/info.py` & `spacy-4.0.0.dev1/spacy/cli/info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Dict, Any, Union, List
 import platform
-import pkg_resources
 import json
 from pathlib import Path
 from wasabi import Printer, MarkdownRenderer
 import srsly
+import importlib.metadata
 
 from ._util import app, Arg, Opt, string_to_list
 from .download import get_model_filename, get_latest_version
 from .. import util
 from .. import about
 
 
@@ -133,23 +133,22 @@
     """Given a pipeline name, get the download URL if available, otherwise
     return None.
 
     This is only available for pipelines installed as modules that have
     dist-info available.
     """
     try:
-        dist = pkg_resources.get_distribution(model)
-        data = json.loads(dist.get_metadata("direct_url.json"))
-        return data["url"]
-    except pkg_resources.DistributionNotFound:
-        # no such package
-        return None
+        dist = importlib.metadata.distribution(model)
+        text = dist.read_text("direct_url.json")
+        if isinstance(text, str):
+            data = json.loads(text)
+            return data["url"]
     except Exception:
-        # something else, like no file or invalid JSON
-        return None
+        pass
+    return None
 
 
 def info_model_url(model: str) -> Dict[str, Any]:
     """Return the download URL for the latest version of a pipeline."""
     version = get_latest_version(model)
 
     filename = get_model_filename(model, version)
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/init_config.py` & `spacy-4.0.0.dev1/spacy/cli/init_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from wasabi import Printer, diff_strings
 from thinc.api import Config
 import srsly
 import re
 from jinja2 import Template
 
 from .. import util
-from ..language import DEFAULT_CONFIG_PRETRAIN_PATH
+from ..language import DEFAULT_CONFIG_DISTILL_PATH, DEFAULT_CONFIG_PRETRAIN_PATH
 from ..schemas import RecommendationSchema
 from ..util import SimpleFrozenList
 from ._util import init_cli, Arg, Opt, show_validation_error, COMMAND
-from ._util import string_to_list, import_code
+from ._util import string_to_list, import_code, _handle_renamed_language_codes
 
 
 ROOT = Path(__file__).parent / "templates"
 TEMPLATE_PATH = ROOT / "quickstart_training.jinja"
 RECOMMENDATIONS = srsly.read_yaml(ROOT / "quickstart_training_recommendations.yml")
 
 
@@ -39,15 +39,15 @@
     force_overwrite = False
 
 
 @init_cli.command("config")
 def init_config_cli(
     # fmt: off
     output_file: Path = Arg(..., help="File to save the config to or - for stdout (will only output config and no additional logging info)", allow_dash=True),
-    lang: str = Opt(InitValues.lang, "--lang", "-l", help="Two-letter code of the language to use"),
+    lang: str = Opt(InitValues.lang, "--lang", "-l", help="Code of the language to use"),
     pipeline: str = Opt(",".join(InitValues.pipeline), "--pipeline", "-p", help="Comma-separated names of trainable pipeline components to include (without 'tok2vec' or 'transformer')"),
     optimize: Optimizations = Opt(InitValues.optimize, "--optimize", "-o", help="Whether to optimize for efficiency (faster inference, smaller model, lower memory consumption) or higher accuracy (potentially larger and slower model). This will impact the choice of architecture, pretrained weights and related hyperparameters."),
     gpu: bool = Opt(InitValues.gpu, "--gpu", "-G", help="Whether the model can run on GPU. This will impact the choice of architecture, pretrained weights and related hyperparameters."),
     pretraining: bool = Opt(InitValues.pretraining, "--pretraining", "-pt", help="Include config for pretraining (with 'spacy pretrain')"),
     force_overwrite: bool = Opt(InitValues.force_overwrite, "--force", "-F", help="Force overwriting the output file"),
     # fmt: on
 ):
@@ -79,14 +79,15 @@
 
 
 @init_cli.command("fill-config")
 def init_fill_config_cli(
     # fmt: off
     base_path: Path = Arg(..., help="Path to base config to fill", exists=True, dir_okay=False),
     output_file: Path = Arg("-", help="Path to output .cfg file (or - for stdout)", allow_dash=True),
+    distillation: bool = Opt(False, "--distillation", "-dt", help="Include config for distillation (with 'spacy distill')"),
     pretraining: bool = Opt(False, "--pretraining", "-pt", help="Include config for pretraining (with 'spacy pretrain')"),
     diff: bool = Opt(False, "--diff", "-D", help="Print a visual diff highlighting the changes"),
     code_path: Optional[Path] = Opt(None, "--code-path", "--code", "-c", help="Path to Python file with additional code (registered functions) to be imported"),
     # fmt: on
 ):
     """
     Fill partial config file with default values. Will add all missing settings
@@ -94,21 +95,28 @@
     functions for their default values and update the base config. This command
     can be used with a config generated via the training quickstart widget:
     https://spacy.io/usage/training#quickstart
 
     DOCS: https://spacy.io/api/cli#init-fill-config
     """
     import_code(code_path)
-    fill_config(output_file, base_path, pretraining=pretraining, diff=diff)
+    fill_config(
+        output_file,
+        base_path,
+        distillation=distillation,
+        pretraining=pretraining,
+        diff=diff,
+    )
 
 
 def fill_config(
     output_file: Path,
     base_path: Path,
     *,
+    distillation: bool = False,
     pretraining: bool = False,
     diff: bool = False,
     silent: bool = False,
 ) -> Tuple[Config, Config]:
     is_stdout = str(output_file) == "-"
     no_print = is_stdout or silent
     msg = Printer(no_print=no_print)
@@ -119,14 +127,17 @@
     # config result is a valid config
     nlp = util.load_model_from_config(nlp.config)
     filled = nlp.config
     # If we have sourced components in the base config, those will have been
     # replaced with their actual config after loading, so we have to re-add them
     sourced = util.get_sourced_components(config)
     filled["components"].update(sourced)
+    if distillation:
+        distillation_config = util.load_config(DEFAULT_CONFIG_DISTILL_PATH)
+        filled = distillation_config.merge(filled)
     if pretraining:
         validate_config_for_pretrain(filled, msg)
         pretrain_config = util.load_config(DEFAULT_CONFIG_PRETRAIN_PATH)
         filled = pretrain_config.merge(filled)
     before = config.to_str()
     after = filled.to_str()
     if before == after:
@@ -154,14 +165,18 @@
     gpu: bool = InitValues.gpu,
     pretraining: bool = InitValues.pretraining,
     silent: bool = True,
 ) -> Config:
     msg = Printer(no_print=silent)
     with TEMPLATE_PATH.open("r") as f:
         template = Template(f.read())
+
+    # Throw error for renamed language codes in v4
+    _handle_renamed_language_codes(lang)
+
     # Filter out duplicates since tok2vec and transformer are added by template
     pipeline = [pipe for pipe in pipeline if pipe not in ("tok2vec", "transformer")]
     defaults = RECOMMENDATIONS["__default__"]
     reco = RecommendationSchema(**RECOMMENDATIONS.get(lang, defaults)).dict()
     variables = {
         "lang": lang,
         "components": pipeline,
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/init_pipeline.py` & `spacy-4.0.0.dev1/spacy/cli/init_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,48 @@
 import typer
 import srsly
 
 from .. import util
 from ..training.initialize import init_nlp, convert_vectors
 from ..language import Language
 from ._util import init_cli, Arg, Opt, parse_config_overrides, show_validation_error
-from ._util import import_code, setup_gpu
+from ._util import import_code, setup_gpu, _handle_renamed_language_codes
 
 
 @init_cli.command("vectors")
 def init_vectors_cli(
     # fmt: off
     lang: str = Arg(..., help="The language of the nlp object to create"),
     vectors_loc: Path = Arg(..., help="Vectors file in Word2Vec format", exists=True),
     output_dir: Path = Arg(..., help="Pipeline output directory"),
     prune: int = Opt(-1, "--prune", "-p", help="Optional number of vectors to prune to"),
     truncate: int = Opt(0, "--truncate", "-t", help="Optional number of vectors to truncate to when reading in vectors file"),
     mode: str = Opt("default", "--mode", "-m", help="Vectors mode: default or floret"),
-    name: Optional[str] = Opt(None, "--name", "-n", help="Optional name for the word vectors, e.g. en_core_web_lg.vectors"),
     verbose: bool = Opt(False, "--verbose", "-V", "-VV", help="Display more information for debugging purposes"),
     jsonl_loc: Optional[Path] = Opt(None, "--lexemes-jsonl", "-j", help="Location of JSONL-formatted attributes file", hidden=True),
     # fmt: on
 ):
     """Convert word vectors for use with spaCy. Will export an nlp object that
     you can use in the [initialize] block of your config to initialize
     a model with vectors.
     """
     util.logger.setLevel(logging.DEBUG if verbose else logging.INFO)
+
+    # Throw error for renamed language codes in v4
+    _handle_renamed_language_codes(lang)
+
     msg.info(f"Creating blank nlp object for language '{lang}'")
     nlp = util.get_lang_class(lang)()
     if jsonl_loc is not None:
         update_lexemes(nlp, jsonl_loc)
     convert_vectors(
         nlp,
         vectors_loc,
         truncate=truncate,
         prune=prune,
-        name=name,
         mode=mode,
     )
     msg.good(f"Successfully converted {len(nlp.vocab.vectors)} vectors")
     nlp.to_disk(output_dir)
     msg.good(
         "Saved nlp object with vectors to output directory. You can now use the "
         "path to it in your config as the 'vectors' setting in [initialize].",
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/package.py` & `spacy-4.0.0.dev1/spacy/cli/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
                 try:
                     func_info = util.registry.find(reg_name, func_name)
                 except RegistryError as regerr:
                     # lang-specific version being absent is not actually an issue
                     raise regerr from None
             module_name = func_info.get("module")  # type: ignore[attr-defined]
             if module_name:  # the code is part of a module, not a --code file
-                modules.add(func_info["module"].split(".")[0])  # type: ignore[index]
+                modules.add(func_info["module"].split(".")[0])  # type: ignore[union-attr]
     dependencies = []
     for module_name in modules:
         if module_name in distributions:
             dist = distributions.get(module_name)
             if dist:
                 pkg = dist[0]
                 if pkg in own_packages or pkg in exclude:
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/pretrain.py` & `spacy-4.0.0.dev1/spacy/cli/pretrain.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     ctx: typer.Context,  # This is only used to read additional arguments
     config_path: Path = Arg(..., help="Path to config file", exists=True, dir_okay=False, allow_dash=True),
     output_dir: Path = Arg(..., help="Directory to write weights to on each epoch"),
     code_path: Optional[Path] = Opt(None, "--code", "-c", help="Path to Python file with additional code (registered functions) to be imported"),
     resume_path: Optional[Path] = Opt(None, "--resume-path", "-r", help="Path to pretrained weights from which to resume pretraining"),
     epoch_resume: Optional[int] = Opt(None, "--epoch-resume", "-er", help="The epoch to resume counting from when using --resume-path. Prevents unintended overwriting of existing weight files."),
     use_gpu: int = Opt(-1, "--gpu-id", "-g", help="GPU ID or -1 for CPU"),
+    skip_last: bool = Opt(False, "--skip-last", "-L", help="Skip saving model-last.bin"),
     # fmt: on
 ):
     """
     Pre-train the 'token-to-vector' (tok2vec) layer of pipeline components,
     using an approximate language-modelling objective. Two objective types
     are available, vector-based and character-based.
 
@@ -70,14 +71,15 @@
     pretrain(
         config,
         output_dir,
         resume_path=resume_path,
         epoch_resume=epoch_resume,
         use_gpu=use_gpu,
         silent=False,
+        skip_last=skip_last,
     )
     msg.good("Successfully finished pretrain")
 
 
 def verify_cli_args(config_path, output_dir, resume_path, epoch_resume):
     if not config_path or (str(config_path) != "-" and not config_path.exists()):
         msg.fail("Config file not found", config_path, exits=1)
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/profile.py` & `spacy-4.0.0.dev1/spacy/cli/profile.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/assets.py` & `spacy-4.0.0.dev1/spacy/cli/project/assets.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/clone.py` & `spacy-4.0.0.dev1/spacy/cli/project/clone.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/document.py` & `spacy-4.0.0.dev1/spacy/cli/project/document.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/dvc.py` & `spacy-4.0.0.dev1/spacy/cli/project/dvc.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/pull.py` & `spacy-4.0.0.dev1/spacy/cli/project/pull.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,30 +35,33 @@
     storage = RemoteStorage(project_dir, remote)
     commands = list(config.get("commands", []))
     # We use a while loop here because we don't know how the commands
     # will be ordered. A command might need dependencies from one that's later
     # in the list.
     while commands:
         for i, cmd in enumerate(list(commands)):
-            logger.debug(f"CMD: {cmd['name']}.")
+            logger.debug("CMD: %s.", cmd["name"])
             deps = [project_dir / dep for dep in cmd.get("deps", [])]
             if all(dep.exists() for dep in deps):
                 cmd_hash = get_command_hash("", "", deps, cmd["script"])
                 for output_path in cmd.get("outputs", []):
                     url = storage.pull(output_path, command_hash=cmd_hash)
                     logger.debug(
-                        f"URL: {url} for {output_path} with command hash {cmd_hash}"
+                        "URL: %s for %s with command hash %s",
+                        url,
+                        output_path,
+                        cmd_hash,
                     )
                     yield url, output_path
 
                 out_locs = [project_dir / out for out in cmd.get("outputs", [])]
                 if all(loc.exists() for loc in out_locs):
                     update_lockfile(project_dir, cmd)
                 # We remove the command from the list here, and break, so that
                 # we iterate over the loop again.
                 commands.pop(i)
                 break
             else:
-                logger.debug(f"Dependency missing. Skipping {cmd['name']} outputs.")
+                logger.debug("Dependency missing. Skipping %s outputs.", cmd["name"])
         else:
             # If we didn't break the for loop, break the while loop.
             break
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/push.py` & `spacy-4.0.0.dev1/spacy/cli/project/push.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,33 +33,33 @@
     library can upload to, e.g. gcs, aws, ssh, local directories etc
     """
     config = load_project_config(project_dir)
     if remote in config.get("remotes", {}):
         remote = config["remotes"][remote]
     storage = RemoteStorage(project_dir, remote)
     for cmd in config.get("commands", []):
-        logger.debug(f"CMD: cmd['name']")
+        logger.debug("CMD: %s", cmd["name"])
         deps = [project_dir / dep for dep in cmd.get("deps", [])]
         if any(not dep.exists() for dep in deps):
-            logger.debug(f"Dependency missing. Skipping {cmd['name']} outputs")
+            logger.debug("Dependency missing. Skipping %s outputs", cmd["name"])
             continue
         cmd_hash = get_command_hash(
             "", "", [project_dir / dep for dep in cmd.get("deps", [])], cmd["script"]
         )
-        logger.debug(f"CMD_HASH: {cmd_hash}")
+        logger.debug("CMD_HASH: %s", cmd_hash)
         for output_path in cmd.get("outputs", []):
             output_loc = project_dir / output_path
             if output_loc.exists() and _is_not_empty_dir(output_loc):
                 url = storage.push(
                     output_path,
                     command_hash=cmd_hash,
                     content_hash=get_content_hash(output_loc),
                 )
                 logger.debug(
-                    f"URL: {url} for output {output_path} with cmd_hash {cmd_hash}"
+                    "URL: %s for output %s with cmd_hash %s", url, output_path, cmd_hash
                 )
                 yield output_path, url
 
 
 def _is_not_empty_dir(loc: Path):
     if not loc.is_dir():
         return True
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/remote_storage.py` & `spacy-4.0.0.dev1/spacy/cli/project/remote_storage.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/project/run.py` & `spacy-4.0.0.dev1/spacy/cli/project/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional, List, Dict, Sequence, Any, Iterable, Tuple
 import os.path
 from pathlib import Path
 
-import pkg_resources
 from wasabi import msg
 from wasabi.util import locale_escape
 import sys
 import srsly
 import typer
 
 from ... import about
@@ -327,14 +326,15 @@
 
 def _check_requirements(requirements: List[str]) -> Tuple[bool, bool]:
     """Checks whether requirements are installed and free of version conflicts.
     requirements (List[str]): List of requirements.
     RETURNS (Tuple[bool, bool]): Whether (1) any packages couldn't be imported, (2) any packages with version conflicts
         exist.
     """
+    import pkg_resources
 
     failed_pkgs_msgs: List[str] = []
     conflicting_pkgs_msgs: List[str] = []
 
     for req in requirements:
         try:
             pkg_resources.require(req)
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/templates/quickstart_training.jinja` & `spacy-4.0.0.dev1/spacy/cli/templates/quickstart_training.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {# This is a template for training configs used for the quickstart widget in
 the docs and the init config command. It encodes various best practices and
 can help generate the best possible configuration, given a user's requirements. #}
 {%- set use_transformer = hardware != "cpu" and transformer_data -%}
 {%- set transformer = transformer_data[optimize] if use_transformer else {} -%}
-{%- set listener_components = ["tagger", "morphologizer", "parser", "ner", "textcat", "textcat_multilabel", "entity_linker", "spancat", "trainable_lemmatizer"] -%}
+{%- set listener_components = ["tagger", "morphologizer", "parser", "ner", "textcat", "textcat_multilabel", "entity_linker", "span_finder", "spancat", "spancat_singlelabel", "trainable_lemmatizer"] -%}
 [paths]
 train = null
 dev = null
 {% if use_transformer or optimize == "efficiency" or not word_vectors -%}
 vectors = null
 {% else -%}
 vectors = "{{ word_vectors }}"
@@ -20,16 +20,19 @@
 gpu_allocator = null
 {% endif %}
 
 [nlp]
 lang = "{{ lang }}"
 {%- set has_textcat = ("textcat" in components or "textcat_multilabel" in components) -%}
 {%- set with_accuracy = optimize == "accuracy" -%}
-{%- set has_accurate_textcat = has_textcat and with_accuracy -%}
-{%- if ("tagger" in components or "morphologizer" in components or "parser" in components or "ner" in components or "spancat" in components or "trainable_lemmatizer" in components or "entity_linker" in components or has_accurate_textcat) -%}
+{# The BOW textcat doesn't need a source of features, so it can omit the
+tok2vec/transformer. #}
+{%- set with_accuracy_or_transformer = (use_transformer or with_accuracy) -%}
+{%- set textcat_needs_features = has_textcat and with_accuracy_or_transformer -%}
+{%- if ("tagger" in components or "morphologizer" in components or "parser" in components or "ner" in components or "span_finder" in components or "spancat" in components or "spancat_singlelabel" in components or "trainable_lemmatizer" in components or "entity_linker" in components or textcat_needs_features) -%}
 {%- set full_pipeline = ["transformer" if use_transformer else "tok2vec"] + components -%}
 {%- else -%}
 {%- set full_pipeline = components -%}
 {%- endif %}
 pipeline = {{ full_pipeline|pprint()|replace("'", '"')|safe }}
 batch_size = {{ 128 if hardware == "gpu" else 1000 }}
 
@@ -118,14 +121,38 @@
 @architectures = "spacy-transformers.TransformerListener.v1"
 grad_factor = 1.0
 
 [components.ner.model.tok2vec.pooling]
 @layers = "reduce_mean.v1"
 {% endif -%}
 
+{% if "span_finder" in components -%}
+[components.span_finder]
+factory = "span_finder"
+max_length = null
+min_length = null
+scorer = {"@scorers":"spacy.span_finder_scorer.v1"}
+spans_key = "sc"
+threshold = 0.5
+
+[components.span_finder.model]
+@architectures = "spacy.SpanFinder.v1"
+
+[components.span_finder.model.scorer]
+@layers = "spacy.LinearLogistic.v1"
+nO = 2
+
+[components.span_finder.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
+
+[components.span_finder.model.tok2vec.pooling]
+@layers = "reduce_mean.v1"
+{% endif -%}
+
 {% if "spancat" in components -%}
 [components.spancat]
 factory = "spancat"
 max_positive = null
 scorer = {"@scorers":"spacy.spancat_scorer.v1"}
 spans_key = "sc"
 threshold = 0.5
@@ -150,14 +177,44 @@
 @layers = "reduce_mean.v1"
 
 [components.spancat.suggester]
 @misc = "spacy.ngram_suggester.v1"
 sizes = [1,2,3]
 {% endif -%}
 
+{% if "spancat_singlelabel" in components %}
+[components.spancat_singlelabel]
+factory = "spancat_singlelabel"
+negative_weight = 1.0
+allow_overlap = true
+scorer = {"@scorers":"spacy.spancat_scorer.v1"}
+spans_key = "sc"
+
+[components.spancat_singlelabel.model]
+@architectures = "spacy.SpanCategorizer.v1"
+
+[components.spancat_singlelabel.model.reducer]
+@layers = "spacy.mean_max_reducer.v1"
+hidden_size = 128
+
+[components.spancat_singlelabel.model.scorer]
+@layers = "Softmax.v2"
+
+[components.spancat_singlelabel.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
+
+[components.spancat_singlelabel.model.tok2vec.pooling]
+@layers = "reduce_mean.v1"
+
+[components.spancat_singlelabel.suggester]
+@misc = "spacy.ngram_suggester.v1"
+sizes = [1,2,3]
+{% endif %}
+
 {% if "trainable_lemmatizer" in components -%}
 [components.trainable_lemmatizer]
 factory = "trainable_lemmatizer"
 backoff = "orth"
 min_tree_freq = 3
 overwrite = false
 scorer = {"@scorers":"spacy.lemmatizer_scorer.v1"}
@@ -215,18 +272,24 @@
 @architectures = "spacy.TextCatBOW.v2"
 exclusive_classes = true
 ngram_size = 1
 no_output_layer = false
 
 {% else -%}
 [components.textcat.model]
-@architectures = "spacy.TextCatBOW.v2"
+@architectures = "spacy.TextCatCNN.v2"
 exclusive_classes = true
-ngram_size = 1
-no_output_layer = false
+nO = null
+
+[components.textcat.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
+
+[components.textcat.model.tok2vec.pooling]
+@layers = "reduce_mean.v1"
 {%- endif %}
 {%- endif %}
 
 {% if "textcat_multilabel" in components %}
 [components.textcat_multilabel]
 factory = "textcat_multilabel"
 
@@ -246,18 +309,24 @@
 @architectures = "spacy.TextCatBOW.v2"
 exclusive_classes = false
 ngram_size = 1
 no_output_layer = false
 
 {% else -%}
 [components.textcat_multilabel.model]
-@architectures = "spacy.TextCatBOW.v2"
+@architectures = "spacy.TextCatCNN.v2"
 exclusive_classes = false
-ngram_size = 1
-no_output_layer = false
+nO = null
+
+[components.textcat_multilabel.model.tok2vec]
+@architectures = "spacy-transformers.TransformerListener.v1"
+grad_factor = 1.0
+
+[components.textcat_multilabel.model.tok2vec.pooling]
+@layers = "reduce_mean.v1"
 {%- endif %}
 {%- endif %}
 
 {# NON-TRANSFORMER PIPELINE #}
 {% else -%}
 {% if "tok2vec" in full_pipeline -%}
 [components.tok2vec]
@@ -280,27 +349,29 @@
 window_size = 1
 maxout_pieces = 3
 {% endif -%}
 
 {% if "morphologizer" in components %}
 [components.morphologizer]
 factory = "morphologizer"
+label_smoothing = 0.05
 
 [components.morphologizer.model]
 @architectures = "spacy.Tagger.v2"
 nO = null
 
 [components.morphologizer.model.tok2vec]
 @architectures = "spacy.Tok2VecListener.v1"
 width = ${components.tok2vec.model.encode.width}
 {%- endif %}
 
 {% if "tagger" in components %}
 [components.tagger]
 factory = "tagger"
+label_smoothing = 0.05
 
 [components.tagger.model]
 @architectures = "spacy.Tagger.v2"
 nO = null
 
 [components.tagger.model.tok2vec]
 @architectures = "spacy.Tok2VecListener.v1"
@@ -337,14 +408,35 @@
 nO = null
 
 [components.ner.model.tok2vec]
 @architectures = "spacy.Tok2VecListener.v1"
 width = ${components.tok2vec.model.encode.width}
 {% endif %}
 
+{% if "span_finder" in components %}
+[components.span_finder]
+factory = "span_finder"
+max_length = null
+min_length = null
+scorer = {"@scorers":"spacy.span_finder_scorer.v1"}
+spans_key = "sc"
+threshold = 0.5
+
+[components.span_finder.model]
+@architectures = "spacy.SpanFinder.v1"
+
+[components.span_finder.model.scorer]
+@layers = "spacy.LinearLogistic.v1"
+nO = 2
+
+[components.span_finder.model.tok2vec]
+@architectures = "spacy.Tok2VecListener.v1"
+width = ${components.tok2vec.model.encode.width}
+{% endif %}
+
 {% if "spancat" in components %}
 [components.spancat]
 factory = "spancat"
 max_positive = null
 scorer = {"@scorers":"spacy.spancat_scorer.v1"}
 spans_key = "sc"
 threshold = 0.5
@@ -366,14 +458,41 @@
 width = ${components.tok2vec.model.encode.width}
 
 [components.spancat.suggester]
 @misc = "spacy.ngram_suggester.v1"
 sizes = [1,2,3]
 {% endif %}
 
+{% if "spancat_singlelabel" in components %}
+[components.spancat_singlelabel]
+factory = "spancat_singlelabel"
+negative_weight = 1.0
+allow_overlap = true
+scorer = {"@scorers":"spacy.spancat_scorer.v1"}
+spans_key = "sc"
+
+[components.spancat_singlelabel.model]
+@architectures = "spacy.SpanCategorizer.v1"
+
+[components.spancat_singlelabel.model.reducer]
+@layers = "spacy.mean_max_reducer.v1"
+hidden_size = 128
+
+[components.spancat_singlelabel.model.scorer]
+@layers = "Softmax.v2"
+
+[components.spancat_singlelabel.model.tok2vec]
+@architectures = "spacy.Tok2VecListener.v1"
+width = ${components.tok2vec.model.encode.width}
+
+[components.spancat_singlelabel.suggester]
+@misc = "spacy.ngram_suggester.v1"
+sizes = [1,2,3]
+{% endif %}
+
 {% if "trainable_lemmatizer" in components -%}
 [components.trainable_lemmatizer]
 factory = "trainable_lemmatizer"
 backoff = "orth"
 min_tree_freq = 3
 overwrite = false
 scorer = {"@scorers":"spacy.lemmatizer_scorer.v1"}
```

### Comparing `spacy-4.0.0.dev0/spacy/cli/templates/quickstart_training_recommendations.yml` & `spacy-4.0.0.dev1/spacy/cli/templates/quickstart_training_recommendations.yml`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/train.py` & `spacy-4.0.0.dev1/spacy/cli/train.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/cli/validate.py` & `spacy-4.0.0.dev1/spacy/cli/validate.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/default_config.cfg` & `spacy-4.0.0.dev1/spacy/default_config.cfg`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/default_config_pretraining.cfg` & `spacy-4.0.0.dev1/spacy/default_config_pretraining.cfg`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/displacy/__init__.py` & `spacy-4.0.0.dev1/spacy/displacy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,15 @@
     """
     from wsgiref import simple_server
 
     port = find_available_port(port, host, auto_select_port)
 
     if is_in_jupyter():
         warnings.warn(Warnings.W011)
-    render(
-        docs, style=style, page=page, minify=minify, options=options, manual=manual
-    )
+    render(docs, style=style, page=page, minify=minify, options=options, manual=manual)
     httpd = simple_server.make_server(host, port, app)
     print(f"\nUsing the '{style}' visualizer")
     print(f"Serving on http://{host}:{port} ...\n")
     try:
         httpd.serve_forever()
     except KeyboardInterrupt:
         print(f"Shutting down server on port {port}.")
@@ -123,21 +121,25 @@
 def app(environ, start_response):
     headers = [("Content-type", "text/html; charset=utf-8")]
     start_response("200 OK", headers)
     res = _html["parsed"].encode(encoding="utf-8")
     return [res]
 
 
-def parse_deps(orig_doc: Doc, options: Dict[str, Any] = {}) -> Dict[str, Any]:
+def parse_deps(
+    orig_doc: Union[Doc, Span], options: Dict[str, Any] = {}
+) -> Dict[str, Any]:
     """Generate dependency parse in {'words': [], 'arcs': []} format.
 
-    orig_doc (Doc): Document to parse.
+    orig_doc (Union[Doc, Span]): Document to parse.
     options (Dict[str, Any]): Dependency parse specific visualisation options.
     RETURNS (dict): Generated dependency parse keyed by words and arcs.
     """
+    if isinstance(orig_doc, Span):
+        orig_doc = orig_doc.as_doc()
     doc = Doc(orig_doc.vocab).from_bytes(
         orig_doc.to_bytes(exclude=["user_data", "user_hooks"])
     )
     if not doc.has_annotation("DEP"):
         warnings.warn(Warnings.W005)
     if options.get("collapse_phrases", False):
         with doc.retokenize() as retokenizer:
```

### Comparing `spacy-4.0.0.dev0/spacy/displacy/render.py` & `spacy-4.0.0.dev1/spacy/displacy/render.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/displacy/templates.py` & `spacy-4.0.0.dev1/spacy/displacy/templates.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/errors.py` & `spacy-4.0.0.dev1/spacy/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from typing import Literal
 import warnings
-from .compat import Literal
 
 
 class ErrorsWithCodes(type):
     def __getattribute__(self, code):
         msg = super().__getattribute__(code)
         if code.startswith("__"):  # python system attributes like __class__
             return msg
@@ -78,15 +78,15 @@
             "try using `nlp.make_doc(text)` or process all texts as a stream "
             "using `list(nlp.tokenizer.pipe(all_texts))`.")
     W017 = ("Alias '{alias}' already exists in the Knowledge Base.")
     W018 = ("Entity '{entity}' already exists in the Knowledge Base - "
             "ignoring the duplicate entry.")
     W021 = ("Unexpected hash collision in PhraseMatcher. Matches may be "
             "incorrect. Modify PhraseMatcher._terminal_hash to fix.")
-    W024 = ("Entity '{entity}' - Alias '{alias}' combination already exists in "
+    W024 = ("Entity '{entity}' - alias '{alias}' combination already exists in "
             "the Knowledge Base.")
     W026 = ("Unable to set all sentence boundaries from dependency parses. If "
             "you are constructing a parse tree incrementally by setting "
             "token.head values, you can probably ignore this warning. Consider "
             "using Doc(words, ..., heads=heads, deps=deps) instead.")
     W027 = ("Found a large training file of {size} bytes. Note that it may "
             "be more efficient to split your training data into multiple "
@@ -205,15 +205,19 @@
     W121 = ("Attempting to trace non-existent method '{method}' in pipe '{pipe}'")
     W122 = ("Couldn't trace method '{method}' in pipe '{pipe}'. This can happen if the pipe class "
             "is a Cython extension type.")
     W123 = ("Argument `enable` with value {enable} does not contain all values specified in the config option "
             "`enabled` ({enabled}). Be aware that this might affect other components in your pipeline.")
     W124 = ("{host}:{port} is already in use, using the nearest available port {serve_port} as an alternative.")
 
+    # v4 warning strings
     W400 = ("`use_upper=False` is ignored, the upper layer is always enabled")
+    W401 = ("`incl_prior is True`, but the selected knowledge base type {kb_type} doesn't support prior probability "
+            "lookups so this setting will be ignored. If your KB does support prior probability lookups, make sure "
+            "to return `True` in `.supports_prior_probs`.")
 
 
 class Errors(metaclass=ErrorsWithCodes):
     E001 = ("No component '{name}' found in pipeline. Available names: {opts}")
     E002 = ("Can't find factory for '{name}' for language {lang} ({lang_code}). "
             "This usually happens when spaCy calls `nlp.{method}` with a custom "
             "component name that's not registered on the current language class. "
@@ -433,16 +437,15 @@
             "`--enable-unicode=ucs4 flag`.")
     E132 = ("The vectors for entities and probabilities for alias '{alias}' "
             "should have equal length, but found {entities_length} and "
             "{probabilities_length} respectively.")
     E133 = ("The sum of prior probabilities for alias '{alias}' should not "
             "exceed 1, but found {sum}.")
     E134 = ("Entity '{entity}' is not defined in the Knowledge Base.")
-    E139 = ("Knowledge base for component '{name}' is empty. Use the methods "
-            "`kb.add_entity` and `kb.add_alias` to add entries.")
+    E139 = ("Knowledge base for component '{name}' is empty.")
     E140 = ("The list of entities, prior probabilities and entity vectors "
             "should be of equal length.")
     E141 = ("Entity vectors should be of length {required} instead of the "
             "provided {found}.")
     E143 = ("Labels for component '{name}' not initialized. This can be fixed "
             "by calling add_label, or by providing a representative batch of "
             "examples to the component's `initialize` method.")
@@ -539,14 +542,16 @@
     E199 = ("Unable to merge 0-length span at `doc[{start}:{end}]`.")
     E200 = ("Can't set {attr} from Span.")
     E202 = ("Unsupported {name} mode '{mode}'. Supported modes: {modes}.")
     E203 = ("If the {name} embedding layer is not updated "
             "during training, make sure to include it in 'annotating components'")
 
     # New errors added in v3.x
+    E850 = ("The PretrainVectors objective currently only supports default or "
+            "floret vectors, not {mode} vectors.")
     E851 = ("The 'textcat' component labels should only have values of 0 or 1, "
             "but found value of '{val}'.")
     E852 = ("The tar file pulled from the remote attempted an unsafe path "
             "traversal.")
     E853 = ("Unsupported component factory name '{name}'. The character '.' is "
             "not permitted in factory names.")
     E854 = ("Unable to set doc.ents. Check that the 'ents_filter' does not "
@@ -919,15 +924,15 @@
              "supported values are: 'I', 'O', 'B' and ''")
     E1026 = ("Edit tree has an invalid format:\n{errors}")
     E1027 = ("AlignmentArray only supports slicing with a step of 1.")
     E1028 = ("AlignmentArray only supports indexing using an int or a slice.")
     E1029 = ("Edit tree cannot be applied to form.")
     E1030 = ("Edit tree identifier out of range.")
     E1031 = ("Could not find gold transition - see logs above.")
-    E1032 = ("`{var}` should not be {forbidden}, but received {value}.")
+    E1032 = ("Span {var} {value} is out of bounds for {obj} with length {length}.")
     E1033 = ("Dimension {name} invalid -- only nO, nF, nP")
     E1034 = ("Node index {i} out of bounds ({length})")
     E1035 = ("Token index {i} out of bounds ({length})")
     E1036 = ("Cannot index into NoneNode")
     E1037 = ("Invalid attribute value '{attr}'.")
     E1038 = ("Invalid JSON input: {message}")
     E1039 = ("The {obj} start or end annotations (start: {start}, end: {end}) "
@@ -945,28 +950,43 @@
              "method in '{name}'. If you want to use this method, make "
              "sure it's overwritten on the subclass.")
     E1046 = ("{cls_name} is an abstract class and cannot be instantiated. If you are looking for spaCy's default "
              "knowledge base, use `InMemoryLookupKB`.")
     E1047 = ("`find_threshold()` only supports components with a `scorer` attribute.")
     E1048 = ("Got '{unexpected}' as console progress bar type, but expected one of the following: {expected}")
     E1049 = ("No available port found for displaCy on host {host}. Please specify an available port "
-             "with `displacy.serve(doc, port)`")
-    E1050 = ("Port {port} is already in use. Please specify an available port with `displacy.serve(doc, port)` "
-             "or use `auto_switch_port=True` to pick an available port automatically.")
+             "with `displacy.serve(doc, port=port)`")
+    E1050 = ("Port {port} is already in use. Please specify an available port with `displacy.serve(doc, port=port)` "
+             "or use `auto_select_port=True` to pick an available port automatically.")
+    E1051 = ("'allow_overlap' can only be False when max_positive is 1, but found 'max_positive': {max_positive}.")
+    E1052 = ("Unable to copy spans: the character offsets for the span at "
+             "index {i} in the span group do not align with the tokenization "
+             "in the target doc.")
+    E1053 = ("Both 'min_length' and 'max_length' should be larger than 0, but found"
+             " 'min_length': {min_length}, 'max_length': {max_length}")
+    E1054 = ("The text, including whitespace, must match between reference and "
+             "predicted docs when training {component}.")
 
     # v4 error strings
     E4000 = ("Expected a Doc as input, but got: '{type}'")
     E4001 = ("Expected input to be one of the following types: ({expected_types}), "
              "but got '{received_type}'")
     E4002 = ("Pipe '{name}' requires a teacher pipe for distillation.")
     E4003 = ("Training examples for distillation must have the exact same tokens in the "
              "reference and predicted docs.")
     E4004 = ("Backprop is not supported when is_train is not set.")
+    E4005 = ("EntityLinker_v1 is not supported in spaCy v4. Update your configuration.")
+    E4006 = ("Expected `entity_id` to be of type {exp_type}, but is of type {found_type}.")
+    E4007 = ("Span {var} {value} must be {op} Span {existing_var} "
+             "{existing_value}.")
+    E4008 = ("Span {pos}_char {value} does not correspond to a token {pos}.")
 
 
+RENAMED_LANGUAGE_CODES = {"xx": "mul", "is": "isl"}
+
 # fmt: on
 
 
 class MatchPatternError(ValueError):
     def __init__(self, key, errors):
         """Custom error for validating match patterns.
```

### Comparing `spacy-4.0.0.dev0/spacy/glossary.py` & `spacy-4.0.0.dev1/spacy/glossary.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/kb/kb.pyx` & `spacy-4.0.0.dev1/spacy/kb/kb.pyx`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # cython: infer_types=True, profile=True
 
 from pathlib import Path
 from typing import Iterable, Tuple, Union
 from cymem.cymem cimport Pool
 
 from .candidate import Candidate
-from ..tokens import Span
+from ..tokens import Span, SpanGroup
 from ..util import SimpleFrozenList
 from ..errors import Errors
 
 
 cdef class KnowledgeBase:
     """A `KnowledgeBase` instance stores unique identifiers for entities and their textual aliases,
     to support entity linking of named entities to real-world concepts.
@@ -26,29 +26,31 @@
                 Errors.E1046.format(cls_name=self.__class__.__name__)
             )
 
         self.vocab = vocab
         self.entity_vector_length = entity_vector_length
         self.mem = Pool()
 
-    def get_candidates_batch(self, mentions: Iterable[Span]) -> Iterable[Iterable[Candidate]]:
+    def get_candidates_batch(self, mentions: SpanGroup) -> Iterable[Iterable[Candidate]]:
         """
-        Return candidate entities for specified texts. Each candidate defines the entity, the original alias,
-        and the prior probability of that alias resolving to that entity.
-        If no candidate is found for a given text, an empty list is returned.
-        mentions (Iterable[Span]): Mentions for which to get candidates.
+        Return candidate entities for a specified Span mention. Each candidate defines at least the entity and the
+        entity's embedding vector. Depending on the KB implementation, further properties - such as the prior
+        probability of the specified mention text resolving to that entity - might be included.
+        If no candidates are found for a given mention, an empty list is returned.
+        mentions (SpanGroup): Mentions for which to get candidates.
         RETURNS (Iterable[Iterable[Candidate]]): Identified candidates.
         """
         return [self.get_candidates(span) for span in mentions]
 
     def get_candidates(self, mention: Span) -> Iterable[Candidate]:
         """
-        Return candidate entities for specified text. Each candidate defines the entity, the original alias,
-        and the prior probability of that alias resolving to that entity.
-        If the no candidate is found for a given text, an empty list is returned.
+        Return candidate entities for a specific mention. Each candidate defines at least the entity and the
+        entity's embedding vector. Depending on the KB implementation, further properties - such as the prior
+        probability of the specified mention text resolving to that entity - might be included.
+        If no candidate is found for the given mention, an empty list is returned.
         mention (Span): Mention for which to get candidates.
         RETURNS (Iterable[Candidate]): Identified candidates.
         """
         raise NotImplementedError(
             Errors.E1045.format(parent="KnowledgeBase", method="get_candidates", name=self.__name__)
         )
 
@@ -102,7 +104,14 @@
         Load KnowledgeBase content from disk.
         path (Union[str, Path]): Target file path.
         exclude (Iterable[str]): List of components to exclude.
         """
         raise NotImplementedError(
             Errors.E1045.format(parent="KnowledgeBase", method="from_disk", name=self.__name__)
         )
+
+    @property
+    def supports_prior_probs(self) -> bool:
+        """RETURNS (bool): Whether this KB type supports looking up prior probabilities for entity mentions."""
+        raise NotImplementedError(
+            Errors.E1045.format(parent="KnowledgeBase", method="supports_prior_probs", name=self.__name__)
+        )
```

### Comparing `spacy-4.0.0.dev0/spacy/kb/kb_in_memory.pxd` & `spacy-4.0.0.dev1/spacy/kb/kb_in_memory.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/kb/kb_in_memory.pyx` & `spacy-4.0.0.dev1/spacy/kb/kb_in_memory.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 from ..tokens import Span
 from ..typedefs cimport hash_t
 from ..errors import Errors, Warnings
 from .. import util
 from ..util import SimpleFrozenList, ensure_path
 from ..vocab cimport Vocab
 from .kb cimport KnowledgeBase
-from .candidate import Candidate as Candidate
+from .candidate import InMemoryCandidate
 
 
 cdef class InMemoryLookupKB(KnowledgeBase):
     """An `InMemoryLookupKB` instance stores unique identifiers for entities and their textual aliases,
     to support entity linking of named entities to real-world concepts.
 
-    DOCS: https://spacy.io/api/kb_in_memory
+    DOCS: https://spacy.io/api/inmemorylookupkb
     """
 
     def __init__(self, Vocab vocab, entity_vector_length):
         """Create an InMemoryLookupKB."""
         super().__init__(vocab, entity_vector_length)
         self._entry_index = PreshMap()
         self._alias_index = PreshMap()
@@ -42,14 +42,17 @@
     def _initialize_vectors(self, int64_t nr_entities):
         self._vectors_table = float_matrix(nr_entities + 1)
 
     def _initialize_aliases(self, int64_t nr_aliases):
         self._alias_index = PreshMap(nr_aliases + 1)
         self._aliases_table = alias_vec(nr_aliases + 1)
 
+    def is_empty(self):
+        return len(self) == 0
+
     def __len__(self):
         return self.get_size_entities()
 
     def get_size_entities(self):
         return len(self._entry_index)
 
     def get_entity_strings(self):
@@ -219,37 +222,41 @@
             alias_entry.entry_indices = entry_indices
 
             probs = alias_entry.probs
             probs.push_back(float(prior_prob))
             alias_entry.probs = probs
             self._aliases_table[alias_index] = alias_entry
 
-    def get_candidates(self, mention: Span) -> Iterable[Candidate]:
-        return self.get_alias_candidates(mention.text)  # type: ignore
+    def get_candidates(self, mention: Span) -> Iterable[InMemoryCandidate]:
+        return self._get_alias_candidates(mention.text)  # type: ignore
 
-    def get_alias_candidates(self, str alias) -> Iterable[Candidate]:
+    def _get_alias_candidates(self, str alias) -> Iterable[InMemoryCandidate]:
         """
         Return candidate entities for an alias. Each candidate defines the entity, the original alias,
         and the prior probability of that alias resolving to that entity.
         If the alias is not known in the KB, and empty list is returned.
         """
         cdef hash_t alias_hash = self.vocab.strings[alias]
         if not alias_hash in self._alias_index:
             return []
         alias_index = <int64_t>self._alias_index.get(alias_hash)
         alias_entry = self._aliases_table[alias_index]
 
-        return [Candidate(kb=self,
-                          entity_hash=self._entries[entry_index].entity_hash,
-                          entity_freq=self._entries[entry_index].freq,
-                          entity_vector=self._vectors_table[self._entries[entry_index].vector_index],
-                          alias_hash=alias_hash,
-                          prior_prob=prior_prob)
-                for (entry_index, prior_prob) in zip(alias_entry.entry_indices, alias_entry.probs)
-                if entry_index != 0]
+        return [
+            InMemoryCandidate(
+                kb=self,
+                entity_hash=self._entries[entry_index].entity_hash,
+                alias_hash=alias_hash,
+                entity_vector=self._vectors_table[self._entries[entry_index].vector_index],
+                prior_prob=prior_prob,
+                entity_freq=self._entries[entry_index].freq
+            )
+            for (entry_index, prior_prob) in zip(alias_entry.entry_indices, alias_entry.probs)
+            if entry_index != 0
+        ]
 
     def get_vector(self, str entity):
         cdef hash_t entity_hash = self.vocab.strings[entity]
 
         # Return an empty list if this entity is unknown in this KB
         if entity_hash not in self._entry_index:
             return [0] * self.entity_vector_length
@@ -272,14 +279,17 @@
         alias_entry = self._aliases_table[alias_index]
         for (entry_index, prior_prob) in zip(alias_entry.entry_indices, alias_entry.probs):
             if self._entries[entry_index].entity_hash == entity_hash:
                 return prior_prob
 
         return 0.0
 
+    def supports_prior_probs(self) -> bool:
+        return True
+
     def to_bytes(self, **kwargs):
         """Serialize the current state to a binary string.
         """
         def serialize_header():
             header = (self.get_size_entities(), self.get_size_aliases(), self.entity_vector_length)
             return srsly.json_dumps(header)
```

### Comparing `spacy-4.0.0.dev0/spacy/lang/am/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/am/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/am/examples.py` & `spacy-4.0.0.dev1/spacy/lang/am/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/am/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/am/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/am/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/am/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/am/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/am/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ar/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ar/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ar/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ar/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ar/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ar/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ar/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ar/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ar/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/ar/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/az/examples.py` & `spacy-4.0.0.dev1/spacy/lang/az/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/az/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/az/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/az/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/az/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bg/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/bg/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bg/examples.py` & `spacy-4.0.0.dev1/spacy/lang/bg/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bg/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/bg/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bg/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/bg/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bg/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/bg/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bn/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/bn/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bn/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/bn/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bn/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/bn/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/bn/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/bn/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ca/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ca/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/ca/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ca/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/ca/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ca/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/ca/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ca/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/ca/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/char_classes.py` & `spacy-4.0.0.dev1/spacy/lang/char_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/cs/examples.py` & `spacy-4.0.0.dev1/spacy/lang/cs/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/cs/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/cs/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/cs/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/cs/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/da/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/examples.py` & `spacy-4.0.0.dev1/spacy/lang/da/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/da/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/da/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/da/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/da/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/da/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/da/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/de/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/de/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/de/examples.py` & `spacy-4.0.0.dev1/spacy/lang/de/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/de/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/de/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/de/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/de/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/de/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/de/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/de/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/de/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/dsb/examples.py` & `spacy-4.0.0.dev1/spacy/lang/dsb/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/dsb/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/dsb/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/el/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/examples.py` & `spacy-4.0.0.dev1/spacy/lang/el/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/get_pos_from_wiktionary.py` & `spacy-4.0.0.dev1/spacy/lang/el/get_pos_from_wiktionary.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/el/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/el/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/el/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/el/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/el/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/el/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/el/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/en/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/examples.py` & `spacy-4.0.0.dev1/spacy/lang/en/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/en/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/en/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/en/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/en/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/en/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/en/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/en/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/es/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/examples.py` & `spacy-4.0.0.dev1/spacy/lang/es/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/es/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/es/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/es/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/es/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/es/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/es/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/es/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/eu/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/eu/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/eu/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/eu/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/fa/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/examples.py` & `spacy-4.0.0.dev1/spacy/lang/fa/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/generate_verbs_exc.py` & `spacy-4.0.0.dev1/spacy/lang/fa/generate_verbs_exc.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/fa/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/fa/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/fa/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fa/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/fa/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/fi/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/examples.py` & `spacy-4.0.0.dev1/spacy/lang/fi/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/fi/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/fi/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/fi/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/fi/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fi/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/fi/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/_tokenizer_exceptions_list.py` & `spacy-4.0.0.dev1/spacy/lang/fr/_tokenizer_exceptions_list.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/examples.py` & `spacy-4.0.0.dev1/spacy/lang/fr/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/fr/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/fr/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/fr/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/fr/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/fr/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/fr/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/fr/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ga/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ga/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ga/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/ga/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ga/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ga/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ga/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/ga/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/grc/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/grc/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/grc/examples.py` & `spacy-4.0.0.dev1/spacy/lang/grc/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/grc/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/grc/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/grc/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/grc/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/grc/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/grc/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/grc/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/grc/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/gu/examples.py` & `spacy-4.0.0.dev1/spacy/lang/gu/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/gu/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/gu/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/he/examples.py` & `spacy-4.0.0.dev1/spacy/lang/he/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/he/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/he/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/he/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/he/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hi/examples.py` & `spacy-4.0.0.dev1/spacy/lang/hi/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hi/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/hi/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hi/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/hi/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hr/lemma_lookup_license.txt` & `spacy-4.0.0.dev1/spacy/lang/hr/lemma_lookup_license.txt`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hr/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/hr/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hsb/examples.py` & `spacy-4.0.0.dev1/spacy/lang/hsb/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hsb/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/hsb/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hu/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/hu/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hu/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/hu/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hu/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/hu/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hu/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/hu/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hy/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/hy/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/hy/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/hy/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/id/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/_tokenizer_exceptions_list.py` & `spacy-4.0.0.dev1/spacy/lang/id/_tokenizer_exceptions_list.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/examples.py` & `spacy-4.0.0.dev1/spacy/lang/id/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/id/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/id/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/id/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/id/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/id/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/id/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/is/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/isl/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/it/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/it/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/it/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/it/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/it/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/it/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/it/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/it/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/it/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/it/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/it/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/it/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ja/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ja/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ja/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ja/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ja/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/ja/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ja/tag_bigram_map.py` & `spacy-4.0.0.dev1/spacy/lang/ja/tag_bigram_map.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ja/tag_map.py` & `spacy-4.0.0.dev1/spacy/lang/ja/tag_map.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ja/tag_orth_map.py` & `spacy-4.0.0.dev1/spacy/lang/ja/tag_orth_map.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/kn/examples.py` & `spacy-4.0.0.dev1/spacy/lang/kn/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/kn/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/kn/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ko/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ko/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ko/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ko/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ko/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ko/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ko/tag_map.py` & `spacy-4.0.0.dev1/spacy/lang/ko/tag_map.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ky/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ky/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ky/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ky/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ky/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/ky/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ky/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ky/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ky/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/ky/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/la/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/la/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lb/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/lb/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lb/examples.py` & `spacy-4.0.0.dev1/spacy/lang/lb/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lb/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/lb/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lb/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/lb/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lb/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/lb/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lb/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/lb/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lg/examples.py` & `spacy-4.0.0.dev1/spacy/lang/lg/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lg/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/lg/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lg/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/lg/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lg/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/lg/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lij/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/lij/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lij/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/lij/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lt/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/lt/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lt/examples.py` & `spacy-4.0.0.dev1/spacy/lang/lt/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lt/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/lt/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lt/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/lt/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lt/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/lt/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/lv/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/lv/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/mk/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/mk/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/mk/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/mk/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/mk/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/mk/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/mk/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/mk/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/mk/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ml/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ml/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ml/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ml/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/mr/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/mr/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nb/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/nb/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nb/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/nb/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nb/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/nb/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nb/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/nb/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nb/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/nb/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ne/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ne/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ne/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ne/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ne/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ne/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/nl/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/nl/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/nl/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/nl/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/nl/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/nl/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/nl/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/nl/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/norm_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/norm_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pl/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/pl/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pl/examples.py` & `spacy-4.0.0.dev1/spacy/lang/pl/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pl/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/pl/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pl/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/pl/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pl/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/pl/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pl/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/pl/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pt/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/pt/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pt/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/pt/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pt/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/pt/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pt/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/pt/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/pt/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/pt/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ro/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ro/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ro/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ro/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ro/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ro/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ro/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/ro/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ro/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ro/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ro/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/ro/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ru/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ru/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ru/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ru/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ru/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/ru/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ru/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ru/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ru/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ru/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ru/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/ru/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sa/examples.py` & `spacy-4.0.0.dev1/spacy/lang/sa/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sa/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/sa/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sa/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/sa/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/si/examples.py` & `spacy-4.0.0.dev1/spacy/lang/si/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/si/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/si/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/si/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/si/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sk/examples.py` & `spacy-4.0.0.dev1/spacy/lang/sk/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sk/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/sk/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sk/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/sk/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sl/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/sl/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sl/examples.py` & `spacy-4.0.0.dev1/spacy/lang/sl/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sl/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/sl/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sl/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/sl/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sl/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/sl/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sl/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/sl/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sq/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/sq/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sr/examples.py` & `spacy-4.0.0.dev1/spacy/lang/sr/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sr/lemma_lookup_licence.txt` & `spacy-4.0.0.dev1/spacy/lang/sr/lemma_lookup_licence.txt`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sr/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/sr/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sr/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/sr/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sr/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/sr/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sv/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/sv/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from thinc.api import Model
 from .tokenizer_exceptions import TOKENIZER_EXCEPTIONS
 from .stop_words import STOP_WORDS
 from .lex_attrs import LEX_ATTRS
 from .syntax_iterators import SYNTAX_ITERATORS
 from ...language import Language, BaseDefaults
 from ...pipeline import Lemmatizer
-
-
-# Punctuation stolen from Danish
-from ..da.punctuation import TOKENIZER_INFIXES, TOKENIZER_SUFFIXES
+from .punctuation import TOKENIZER_INFIXES, TOKENIZER_SUFFIXES
 
 
 class SwedishDefaults(BaseDefaults):
     tokenizer_exceptions = TOKENIZER_EXCEPTIONS
     infixes = TOKENIZER_INFIXES
     suffixes = TOKENIZER_SUFFIXES
     lex_attr_getters = LEX_ATTRS
```

### Comparing `spacy-4.0.0.dev0/spacy/lang/sv/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/sv/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sv/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/sv/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sv/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/sv/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/sv/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/sv/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ta/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ta/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ta/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ta/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ta/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ta/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/te/examples.py` & `spacy-4.0.0.dev1/spacy/lang/te/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/te/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/te/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/te/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/te/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/th/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/th/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/th/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/th/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/th/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/th/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/th/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/th/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ti/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/ti/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ti/examples.py` & `spacy-4.0.0.dev1/spacy/lang/ti/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ti/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ti/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ti/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/ti/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ti/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ti/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tl/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/tl/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tl/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/tl/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tl/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/tl/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tn/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/tn/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tn/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/tn/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tn/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/tn/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tr/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/tr/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tr/examples.py` & `spacy-4.0.0.dev1/spacy/lang/tr/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tr/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/tr/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tr/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/tr/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tr/syntax_iterators.py` & `spacy-4.0.0.dev1/spacy/lang/tr/syntax_iterators.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tr/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/tr/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tt/examples.py` & `spacy-4.0.0.dev1/spacy/lang/tt/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tt/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/tt/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tt/punctuation.py` & `spacy-4.0.0.dev1/spacy/lang/tt/punctuation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tt/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/tt/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/tt/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/tt/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/uk/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/uk/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/uk/examples.py` & `spacy-4.0.0.dev1/spacy/lang/uk/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/uk/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/lang/uk/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/uk/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/uk/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/uk/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/uk/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/uk/tokenizer_exceptions.py` & `spacy-4.0.0.dev1/spacy/lang/uk/tokenizer_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ur/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/ur/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/ur/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/ur/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/vi/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/vi/examples.py` & `spacy-4.0.0.dev1/spacy/lang/vi/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/vi/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/vi/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/vi/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/vi/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/xx/examples.py` & `spacy-4.0.0.dev1/spacy/lang/mul/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/yo/examples.py` & `spacy-4.0.0.dev1/spacy/lang/yo/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/yo/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/yo/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/yo/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/yo/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/zh/__init__.py` & `spacy-4.0.0.dev1/spacy/lang/zh/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/zh/examples.py` & `spacy-4.0.0.dev1/spacy/lang/zh/examples.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/zh/lex_attrs.py` & `spacy-4.0.0.dev1/spacy/lang/zh/lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lang/zh/stop_words.py` & `spacy-4.0.0.dev1/spacy/lang/zh/stop_words.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/language.py` & `spacy-4.0.0.dev1/spacy/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import Iterator, Optional, Any, Dict, Callable, Iterable
+from typing import Iterator, Optional, Any, Dict, Callable, Iterable, Literal
 from typing import Union, Tuple, List, Set, Pattern, Sequence
-from typing import NoReturn, TYPE_CHECKING, TypeVar, cast, overload
+from typing import NoReturn, TypeVar, cast, overload
 
 from dataclasses import dataclass
 import random
 import itertools
 import functools
 from contextlib import contextmanager
 from copy import deepcopy
@@ -18,15 +18,15 @@
 from timeit import default_timer as timer
 import traceback
 
 from . import ty
 from .tokens.underscore import Underscore
 from .vocab import Vocab, create_vocab
 from .pipe_analysis import validate_attrs, analyze_pipes, print_pipe_analysis
-from .training import Example, validate_examples
+from .training import Example, validate_examples, validate_distillation_examples
 from .training.initialize import init_vocab, init_tok2vec
 from .scorer import Scorer
 from .util import registry, SimpleFrozenList, _pipe, raise_error, _DEFAULT_EMPTY_PIPES
 from .util import SimpleFrozenDict, combine_score_weights, CONFIG_SECTION_ORDER
 from .util import warn_if_jupyter_cupy
 from .lang.tokenizer_exceptions import URL_MATCH, BASE_EXCEPTIONS
 from .lang.punctuation import TOKENIZER_PREFIXES, TOKENIZER_SUFFIXES
@@ -36,23 +36,25 @@
 from .errors import Errors, Warnings
 from .schemas import ConfigSchema, ConfigSchemaNlp, ConfigSchemaInit
 from .schemas import ConfigSchemaPretrain, validate_init_settings
 from .git_info import GIT_VERSION
 from . import util
 from . import about
 from .lookups import load_lookups
-from .compat import Literal
 
 
 PipeCallable = Callable[[Doc], Doc]
 
 
 # This is the base config will all settings (training etc.)
 DEFAULT_CONFIG_PATH = Path(__file__).parent / "default_config.cfg"
 DEFAULT_CONFIG = util.load_config(DEFAULT_CONFIG_PATH)
+# This is the base config for the [distillation] block and currently not included
+# in the main config and only added via the 'init fill-config' command
+DEFAULT_CONFIG_DISTILL_PATH = Path(__file__).parent / "default_config_distillation.cfg"
 # This is the base config for the [pretraining] block and currently not included
 # in the main config and only added via the 'init fill-config' command
 DEFAULT_CONFIG_PRETRAIN_PATH = Path(__file__).parent / "default_config_pretraining.cfg"
 
 # Type variable for contexts piped with documents
 _AnyContext = TypeVar("_AnyContext")
 
@@ -100,15 +102,15 @@
         )
 
     return tokenizer_factory
 
 
 @registry.misc("spacy.LookupsDataLoader.v1")
 def load_lookups_data(lang, tables):
-    util.logger.debug(f"Loading lookups from spacy-lookups-data: {tables}")
+    util.logger.debug("Loading lookups from spacy-lookups-data: %s", tables)
     lookups = load_lookups(lang=lang, tables=tables)
     return lookups
 
 
 class Language:
     """A text-processing pipeline. Usually you'll load this once per process,
     and pass the instance around your application.
@@ -168,16 +170,15 @@
         # Component meta and configs are only needed on the instance
         self._pipe_meta: Dict[str, "FactoryMeta"] = {}  # meta by component
         self._pipe_configs: Dict[str, Config] = {}  # config by component
 
         if not isinstance(vocab, Vocab) and vocab is not True:
             raise ValueError(Errors.E918.format(vocab=vocab, vocab_type=type(Vocab)))
         if vocab is True:
-            vectors_name = meta.get("vectors", {}).get("name")
-            vocab = create_vocab(self.lang, self.Defaults, vectors_name=vectors_name)
+            vocab = create_vocab(self.lang, self.Defaults)
         else:
             if (self.lang and vocab.lang) and (self.lang != vocab.lang):
                 raise ValueError(Errors.E150.format(nlp=self.lang, vocab=vocab.lang))
         self.vocab: Vocab = vocab
         if self.lang is None:
             self.lang = self.vocab.lang
         self._components: List[Tuple[str, PipeCallable]] = []
@@ -223,15 +224,14 @@
         self._meta.setdefault("url", "")
         self._meta.setdefault("license", "")
         self._meta.setdefault("spacy_git_version", GIT_VERSION)
         self._meta["vectors"] = {
             "width": self.vocab.vectors_length,
             "vectors": len(self.vocab.vectors),
             "keys": self.vocab.vectors.n_keys,
-            "name": self.vocab.vectors.name,
             "mode": self.vocab.vectors.mode,
         }
         self._meta["labels"] = dict(self.pipe_labels)
         # TODO: Adding this back to prevent breaking people's code etc., but
         # we should consider removing it
         self._meta["pipeline"] = list(self.pipe_names)
         self._meta["components"] = list(self.component_names)
@@ -1014,14 +1014,124 @@
                 raise ValueError(Errors.E109.format(name=name)) from e
             except Exception as e:
                 error_handler(name, proc, [doc], e)
             if not isinstance(doc, Doc):
                 raise ValueError(Errors.E005.format(name=name, returned_type=type(doc)))
         return doc
 
+    def distill(
+        self,
+        teacher: "Language",
+        examples: Iterable[Example],
+        *,
+        drop: float = 0.0,
+        sgd: Union[Optimizer, None, Literal[False]] = None,
+        losses: Optional[Dict[str, float]] = None,
+        component_cfg: Optional[Dict[str, Dict[str, Any]]] = None,
+        exclude: Iterable[str] = SimpleFrozenList(),
+        annotates: Iterable[str] = SimpleFrozenList(),
+        student_to_teacher: Optional[Dict[str, str]] = None,
+    ):
+        """Distill the models in a student pipeline from a teacher pipeline.
+        teacher (Language): Teacher to distill from.
+        examples (Iterable[Example]): Distillation examples. The reference
+            (teacher) and predicted (student) docs must have the same number of
+            tokens and the same orthography.
+        drop (float): The dropout rate.
+        sgd (Union[Optimizer, None, Literal[False]]): An optimizer. Will
+            be created via create_optimizer if 'None'. No optimizer will
+            be used when set to 'False'.
+        losses (Optional(Dict[str, float])): Dictionary to update with the loss,
+            keyed by component.
+        component_cfg (Optional[Dict[str, Dict[str, Any]]]): Config parameters
+            for specific pipeline components, keyed by component name.
+        exclude (Iterable[str]): Names of components that shouldn't be updated.
+        annotates (Iterable[str]): Names of components that should set
+            annotations on the predicted examples after updating.
+        student_to_teacher (Optional[Dict[str, str]]): Map student pipe name to
+            teacher pipe name, only needed for pipes where the student pipe
+            name does not match the teacher pipe name.
+        RETURNS (Dict[str, float]): The updated losses dictionary
+
+        DOCS: https://spacy.io/api/language#distill
+        """
+        if student_to_teacher is None:
+            student_to_teacher = {}
+        if losses is None:
+            losses = {}
+        if isinstance(examples, list) and len(examples) == 0:
+            return losses
+
+        validate_distillation_examples(examples, "Language.distill")
+        examples = _copy_examples(examples, copy_x=True, copy_y=True)
+
+        if sgd is None:
+            if self._optimizer is None:
+                self._optimizer = self.create_optimizer()
+            sgd = self._optimizer
+
+        if component_cfg is None:
+            component_cfg = {}
+        pipe_kwargs = {}
+        for student_name, student_proc in self.pipeline:
+            component_cfg.setdefault(student_name, {})
+            pipe_kwargs[student_name] = deepcopy(component_cfg[student_name])
+            component_cfg[student_name].setdefault("drop", drop)
+            pipe_kwargs[student_name].setdefault("batch_size", self.batch_size)
+
+        teacher_pipes = dict(teacher.pipeline)
+        for student_name, student_proc in self.pipeline:
+            if student_name in annotates:
+                for doc, eg in zip(
+                    _pipe(
+                        (eg.predicted for eg in examples),
+                        proc=student_proc,
+                        name=student_name,
+                        default_error_handler=self.default_error_handler,
+                        kwargs=pipe_kwargs[student_name],
+                    ),
+                    examples,
+                ):
+                    eg.predicted = doc
+
+            if (
+                student_name not in exclude
+                and isinstance(student_proc, ty.DistillableComponent)
+                and student_proc.is_distillable
+            ):
+                # A missing teacher pipe is not an error, some student pipes
+                # do not need a teacher, such as tok2vec layer losses.
+                teacher_name = (
+                    student_to_teacher[student_name]
+                    if student_name in student_to_teacher
+                    else student_name
+                )
+                teacher_pipe = teacher_pipes.get(teacher_name, None)
+                student_proc.distill(
+                    teacher_pipe,
+                    examples,
+                    sgd=None,
+                    losses=losses,
+                    **component_cfg[student_name],
+                )
+
+        # Only finish the update after all component updates are done. Some
+        # components may share weights (such as tok2vec) and we only want
+        # to apply weight updates after all gradients are accumulated.
+        for student_name, student_proc in self.pipeline:
+            if (
+                student_name not in exclude
+                and isinstance(student_proc, ty.DistillableComponent)
+                and student_proc.is_distillable
+                and sgd not in (None, False)
+            ):
+                student_proc.finish_update(sgd)
+
+        return losses
+
     def disable_pipes(self, *names) -> "DisabledPipes":
         """Disable one or more pipeline components. If used as a context
         manager, the pipeline will be restored to the initial state at the end
         of the block. Otherwise, a DisabledPipes object is returned, that has
         a `.restore()` method you can use to undo your changes.
 
         This method has been deprecated since 3.0
@@ -1102,26 +1212,28 @@
 
     def update(
         self,
         examples: Iterable[Example],
         _: Optional[Any] = None,
         *,
         drop: float = 0.0,
-        sgd: Optional[Optimizer] = None,
+        sgd: Union[Optimizer, None, Literal[False]] = None,
         losses: Optional[Dict[str, float]] = None,
         component_cfg: Optional[Dict[str, Dict[str, Any]]] = None,
         exclude: Iterable[str] = SimpleFrozenList(),
         annotates: Iterable[str] = SimpleFrozenList(),
     ):
         """Update the models in the pipeline.
 
         examples (Iterable[Example]): A batch of examples
         _: Should not be set - serves to catch backwards-incompatible scripts.
         drop (float): The dropout rate.
-        sgd (Optimizer): An optimizer.
+        sgd (Union[Optimizer, None, Literal[False]]): An optimizer. Will
+            be created via create_optimizer if 'None'. No optimizer will
+            be used when set to 'False'.
         losses (Dict[str, float]): Dictionary to update with the loss, keyed by
             component.
         component_cfg (Dict[str, Dict]): Config parameters for specific pipeline
             components, keyed by component name.
         exclude (Iterable[str]): Names of components that shouldn't be updated.
         annotates (Iterable[str]): Names of components that should set
             annotations on the predicted examples after updating.
@@ -1146,37 +1258,44 @@
         pipe_kwargs = {}
         for i, (name, proc) in enumerate(self.pipeline):
             component_cfg.setdefault(name, {})
             pipe_kwargs[name] = deepcopy(component_cfg[name])
             component_cfg[name].setdefault("drop", drop)
             pipe_kwargs[name].setdefault("batch_size", self.batch_size)
         for name, proc in self.pipeline:
-            # ignore statements are used here because mypy ignores hasattr
-            if name not in exclude and hasattr(proc, "update"):
-                proc.update(examples, sgd=None, losses=losses, **component_cfg[name])  # type: ignore
-            if sgd not in (None, False):
-                if (
-                    name not in exclude
-                    and isinstance(proc, ty.TrainableComponent)
-                    and proc.is_trainable
-                    and proc.model not in (True, False, None)
-                ):
-                    proc.finish_update(sgd)
+            if (
+                name not in exclude
+                and isinstance(proc, ty.TrainableComponent)
+                and proc.is_trainable
+            ):
+                proc.update(examples, sgd=None, losses=losses, **component_cfg[name])
             if name in annotates:
                 for doc, eg in zip(
                     _pipe(
                         (eg.predicted for eg in examples),
                         proc=proc,
                         name=name,
                         default_error_handler=self.default_error_handler,
                         kwargs=pipe_kwargs[name],
                     ),
                     examples,
                 ):
                     eg.predicted = doc
+        # Only finish the update after all component updates are done. Some
+        # components may share weights (such as tok2vec) and we only want
+        # to apply weight updates after all gradients are accumulated.
+        for name, proc in self.pipeline:
+            if (
+                name not in exclude
+                and isinstance(proc, ty.TrainableComponent)
+                and proc.is_trainable
+                and sgd not in (None, False)
+            ):
+                proc.finish_update(sgd)
+
         return losses
 
     def rehearse(
         self,
         examples: Iterable[Example],
         *,
         sgd: Optional[Optimizer] = None,
@@ -1239,32 +1358,39 @@
             sgd(key, W, dW)  # type: ignore[call-arg, misc]
         return losses
 
     def initialize(
         self,
         get_examples: Optional[Callable[[], Iterable[Example]]] = None,
         *,
+        labels: Optional[Dict[str, Any]] = None,
         sgd: Optional[Optimizer] = None,
     ) -> Optimizer:
         """Initialize the pipe for training, using data examples if available.
 
         get_examples (Callable[[], Iterable[Example]]): Optional function that
             returns gold-standard Example objects.
+        labels (Optional[Dict[str, Any]]): Labels to pass to pipe initialization,
+            using the names of the pipes as keys. Overrides labels that are in
+            the model configuration.
         sgd (Optional[Optimizer]): An optimizer to use for updates. If not
             provided, will be created using the .create_optimizer() method.
         RETURNS (thinc.api.Optimizer): The optimizer.
 
         DOCS: https://spacy.io/api/language#initialize
         """
         if get_examples is None:
             util.logger.debug(
                 "No 'get_examples' callback provided to 'Language.initialize', creating dummy examples"
             )
             doc = Doc(self.vocab, words=["x", "y", "z"])
-            get_examples = lambda: [Example.from_dict(doc, {})]
+
+            def get_examples():
+                return [Example.from_dict(doc, {})]
+
         if not hasattr(get_examples, "__call__"):
             err = Errors.E930.format(
                 method="Language.initialize", obj=type(get_examples)
             )
             raise TypeError(err)
         # Make sure the config is interpolated so we can resolve subsections
         config = self.config.interpolate()
@@ -1289,14 +1415,16 @@
                 section="tokenizer",
                 name="tokenizer",
             )
             self.tokenizer.initialize(get_examples, nlp=self, **tok_settings)  # type: ignore[union-attr]
         for name, proc in self.pipeline:
             if isinstance(proc, ty.InitializableComponent):
                 p_settings = I["components"].get(name, {})
+                if labels is not None and name in labels:
+                    p_settings["labels"] = labels[name]
                 p_settings = validate_init_settings(
                     proc.initialize, p_settings, section="components", name=name
                 )
                 proc.initialize(get_examples, nlp=self, **p_settings)
         pretrain_cfg = config.get("pretraining")
         if pretrain_cfg:
             P = registry.resolve(pretrain_cfg, schema=ConfigSchemaPretrain)
@@ -1359,25 +1487,28 @@
         self,
         examples: Iterable[Example],
         *,
         batch_size: Optional[int] = None,
         scorer: Optional[Scorer] = None,
         component_cfg: Optional[Dict[str, Dict[str, Any]]] = None,
         scorer_cfg: Optional[Dict[str, Any]] = None,
+        per_component: bool = False,
     ) -> Dict[str, Any]:
         """Evaluate a model's pipeline components.
 
         examples (Iterable[Example]): `Example` objects.
         batch_size (Optional[int]): Batch size to use.
         scorer (Optional[Scorer]): Scorer to use. If not passed in, a new one
             will be created.
         component_cfg (dict): An optional dictionary with extra keyword
             arguments for specific components.
         scorer_cfg (dict): An optional dictionary with extra keyword arguments
             for the scorer.
+        per_component (bool): Whether to return the scores keyed by component
+            name. Defaults to False.
 
         RETURNS (Scorer): The scorer containing the evaluation results.
 
         DOCS: https://spacy.io/api/language#evaluate
         """
         examples = list(examples)
         validate_examples(examples, "Language.evaluate")
@@ -1402,15 +1533,15 @@
             (eg.predicted for eg in examples),
             batch_size=batch_size,
             component_cfg=component_cfg,
         )
         for eg, doc in zip(examples, docs):
             eg.predicted = doc
         end_time = timer()
-        results = scorer.score(examples)
+        results = scorer.score(examples, per_component=per_component)
         n_words = sum(len(eg.predicted) for eg in examples)
         results["speed"] = n_words / (end_time - start_time)
         return results
 
     def create_optimizer(self):
         """Create an optimizer, usually using the [training.optimizer] config."""
         subconfig = {"optimizer": self.config["training"]["optimizer"]}
@@ -1722,22 +1853,26 @@
         config["nlp"]["lang"] = cls.lang
         # This isn't very elegant, but we remove the [components] block here to prevent
         # it from getting resolved (causes problems because we expect to pass in
         # the nlp and name args for each component). If we're auto-filling, we're
         # using the nlp.config with all defaults.
         config = util.copy_config(config)
         orig_pipeline = config.pop("components", {})
+        orig_distill = config.pop("distillation", None)
         orig_pretraining = config.pop("pretraining", None)
         config["components"] = {}
         if auto_fill:
             filled = registry.fill(config, validate=validate, schema=ConfigSchema)
         else:
             filled = config
         filled["components"] = orig_pipeline
         config["components"] = orig_pipeline
+        if orig_distill is not None:
+            filled["distillation"] = orig_distill
+            config["distillation"] = orig_distill
         if orig_pretraining is not None:
             filled["pretraining"] = orig_pretraining
             config["pretraining"] = orig_pretraining
         resolved_nlp = registry.resolve(
             filled["nlp"], validate=validate, schema=ConfigSchemaNlp
         )
         create_tokenizer = resolved_nlp["tokenizer"]
@@ -1956,15 +2091,15 @@
         if not isinstance(tok2vec, ty.ListenedToComponent):
             raise ValueError(Errors.E888.format(name=tok2vec_name, pipe=type(tok2vec)))
         tok2vec_model = tok2vec.model
         pipe_listeners = tok2vec.listener_map.get(pipe_name, [])
         pipe = self.get_pipe(pipe_name)
         pipe_cfg = self._pipe_configs[pipe_name]
         if listeners:
-            util.logger.debug(f"Replacing listeners of component '{pipe_name}'")
+            util.logger.debug("Replacing listeners of component '%s'", pipe_name)
             if len(list(listeners)) != len(pipe_listeners):
                 # The number of listeners defined in the component model doesn't
                 # match the listeners to replace, so we won't be able to update
                 # the nodes and generate a matching config
                 err = Errors.E887.format(
                     name=pipe_name,
                     tok2vec=tok2vec_name,
@@ -2079,17 +2214,14 @@
         DOCS: https://spacy.io/api/language#from_disk
         """
 
         def deserialize_meta(path: Path) -> None:
             if path.exists():
                 data = srsly.read_json(path)
                 self.meta.update(data)
-                # self.meta always overrides meta["vectors"] with the metadata
-                # from self.vocab.vectors, so set the name directly
-                self.vocab.vectors.name = data.get("vectors", {}).get("name")
 
         def deserialize_vocab(path: Path) -> None:
             if path.exists():
                 self.vocab.from_disk(path, exclude=exclude)
 
         path = util.ensure_path(path)
         deserializers = {}
@@ -2150,17 +2282,14 @@
 
         DOCS: https://spacy.io/api/language#from_bytes
         """
 
         def deserialize_meta(b):
             data = srsly.json_loads(b)
             self.meta.update(data)
-            # self.meta always overrides meta["vectors"] with the metadata
-            # from self.vocab.vectors, so set the name directly
-            self.vocab.vectors.name = data.get("vectors", {}).get("name")
 
         deserializers: Dict[str, Callable[[bytes], Any]] = {}
         deserializers["config.cfg"] = lambda b: self.config.from_bytes(
             b, interpolate=False
         )
         deserializers["meta.json"] = deserialize_meta
         deserializers["vocab"] = lambda b: self.vocab.from_bytes(b, exclude=exclude)
@@ -2219,21 +2348,26 @@
         for name in self.names:
             if name not in self.nlp.component_names:
                 raise ValueError(Errors.E008.format(name=name))
             self.nlp.enable_pipe(name)
         self[:] = []
 
 
-def _copy_examples(examples: Iterable[Example]) -> List[Example]:
+def _copy_examples(
+    examples: Iterable[Example], *, copy_x: bool = True, copy_y: bool = False
+) -> List[Example]:
     """Make a copy of a batch of examples, copying the predicted Doc as well.
     This is used in contexts where we need to take ownership of the examples
     so that they can be mutated, for instance during Language.evaluate and
     Language.update.
     """
-    return [Example(eg.x.copy(), eg.y) for eg in examples]
+    return [
+        Example(eg.x.copy() if copy_x else eg.x, eg.y.copy() if copy_y else eg.y)
+        for eg in examples
+    ]
 
 
 def _apply_pipes(
     ensure_doc: Callable[[Union[str, Doc, bytes], _AnyContext], Doc],
     pipes: Iterable[Callable[..., Iterator[Doc]]],
     receiver,
     sender,
```

### Comparing `spacy-4.0.0.dev0/spacy/lexeme.pxd` & `spacy-4.0.0.dev1/spacy/lexeme.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/lexeme.pyi` & `spacy-4.0.0.dev1/spacy/lexeme.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     def vector_norm(self) -> float: ...
     vector: Floats1d
     rank: int
     @property
     def orth_(self) -> str: ...
     @property
     def text(self) -> str: ...
-    lower: str
+    orth: int
+    lower: int
     norm: int
     shape: int
     prefix: int
     suffix: int
     cluster: int
     lang: int
     prob: float
```

### Comparing `spacy-4.0.0.dev0/spacy/lexeme.pyx` & `spacy-4.0.0.dev1/spacy/lexeme.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         vocab (Vocab): The parent vocabulary
         orth (uint64): The orth id of the lexeme.
         Returns (Lexeme): The newly constructd object.
         """
         self.vocab = vocab
         self.orth = orth
-        self.c = <LexemeC*><void*>vocab.get_by_orth(vocab.mem, orth)
+        self.c = <LexemeC*><void*>vocab.get_by_orth(orth)
         if self.c.orth != orth:
             raise ValueError(Errors.E071.format(orth=orth, vocab_orth=self.c.orth))
 
     def __richcmp__(self, other, int op):
         if other is None:
             if op == 0 or op == 1 or op == 2:
                 return False
@@ -182,15 +182,15 @@
 
     @property
     def text(self):
         """RETURNS (str): The original verbatim text of the lexeme."""
         return self.orth_
 
     property lower:
-        """RETURNS (str): Lowercase form of the lexeme."""
+        """RETURNS (uint64): Lowercase form of the lexeme."""
         def __get__(self):
             return self.c.lower
 
         def __set__(self, attr_t x):
             self.c.lower = x
 
     property norm:
```

### Comparing `spacy-4.0.0.dev0/spacy/lookups.py` & `spacy-4.0.0.dev1/spacy/lookups.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/matcher/dependencymatcher.pyi` & `spacy-4.0.0.dev1/spacy/matcher/dependencymatcher.pyi`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/matcher/dependencymatcher.pyx` & `spacy-4.0.0.dev1/spacy/matcher/dependencymatcher.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,20 @@
             ".*": self._precede,
             ";": self._imm_follow,
             ";*": self._follow,
             "$+": self._imm_right_sib,
             "$-": self._imm_left_sib,
             "$++": self._right_sib,
             "$--": self._left_sib,
+            ">+": self._imm_right_child,
+            ">-": self._imm_left_child,
             ">++": self._right_child,
             ">--": self._left_child,
+            "<+": self._imm_right_parent,
+            "<-": self._imm_left_parent,
             "<++": self._right_parent,
             "<--": self._left_parent,
         }
 
     def __reduce__(self):
         data = (self.vocab, self._raw_patterns, self._callbacks)
         return (unpickle_matcher, data, None, None)
@@ -423,19 +427,41 @@
 
     def _right_sib(self, doc, node):
         return [doc[child.i] for child in doc[node].head.children if child.i > node]
 
     def _left_sib(self, doc, node):
         return [doc[child.i] for child in doc[node].head.children if child.i < node]
 
+    def _imm_right_child(self, doc, node):
+        for child in doc[node].rights:
+            if child.i == node + 1:
+                return [doc[child.i]]
+        return []
+
+    def _imm_left_child(self, doc, node):
+        for child in doc[node].lefts:
+            if child.i == node - 1:
+                return [doc[child.i]]
+        return []
+
     def _right_child(self, doc, node):
-        return [doc[child.i] for child in doc[node].children if child.i > node]
+        return [child for child in doc[node].rights]
     
     def _left_child(self, doc, node):
-        return [doc[child.i] for child in doc[node].children if child.i < node]
+        return [child for child in doc[node].lefts]
+
+    def _imm_right_parent(self, doc, node):
+        if doc[node].head.i == node + 1:
+            return [doc[node].head]
+        return []
+
+    def _imm_left_parent(self, doc, node):
+        if doc[node].head.i == node - 1:
+            return [doc[node].head]
+        return []
 
     def _right_parent(self, doc, node):
         if doc[node].head.i > node:
             return [doc[node].head]
         return []
     
     def _left_parent(self, doc, node):
```

### Comparing `spacy-4.0.0.dev0/spacy/matcher/levenshtein.c` & `spacy-4.0.0.dev1/spacy/matcher/levenshtein.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/opt/hostedtoolcache/Python/3.8.15/x64/include/python3.8/Python.h",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/include/python3.8/Python.h",
             "spacy/matcher/polyleven.c"
         ],
         "include_dirs": [
             "spacy/matcher",
-            "/opt/hostedtoolcache/Python/3.8.15/x64/lib/python3.8/site-packages/numpy/core/include",
-            "/opt/hostedtoolcache/Python/3.8.15/x64/include/python3.8"
+            "/tmp/build-env-z_27ltsx/lib/python3.8/site-packages/numpy/core/include",
+            "/opt/hostedtoolcache/Python/3.8.17/x64/include/python3.8"
         ],
         "language": "c",
         "name": "spacy.matcher.levenshtein",
         "sources": [
             "spacy/matcher/levenshtein.pyx",
             "spacy/matcher/polyleven.c"
         ]
@@ -28,16 +28,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -97,16 +97,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -222,15 +226,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -261,15 +265,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1465,22 +1469,30 @@
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -2000,15 +2012,15 @@
  *     else:
  */
     goto __pyx_L3;
   }
 
   /* "spacy/matcher/levenshtein.pyx":26
  *         # allow at least two edits (to allow at least one transposition) and up
- *         # to 20% of the pattern string length
+ *         # to 30% of the pattern string length
  *         max_edits = max(2, round(0.3 * len(pattern_text)))             # <<<<<<<<<<<<<<
  *     return levenshtein(input_text, pattern_text, max_edits) <= max_edits
  * 
  */
   /*else*/ {
     __pyx_t_3 = PyObject_Length(__pyx_v_pattern_text); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 26, __pyx_L1_error)
     __pyx_t_1 = PyFloat_FromDouble((0.3 * __pyx_t_3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
@@ -2038,15 +2050,15 @@
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_v_max_edits = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "spacy/matcher/levenshtein.pyx":27
- *         # to 20% of the pattern string length
+ *         # to 30% of the pattern string length
  *         max_edits = max(2, round(0.3 * len(pattern_text)))
  *     return levenshtein(input_text, pattern_text, max_edits) <= max_edits             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_9.__pyx_n = 1;
   __pyx_t_9.k = __pyx_v_max_edits;
@@ -2451,22 +2463,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3476,61 +3487,79 @@
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -4349,15 +4378,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -4710,15 +4742,15 @@
                         } else if (8 * sizeof(int64_t) >= 4 * PyLong_SHIFT) {
                             return (int64_t) (((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -4982,15 +5014,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5178,15 +5210,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `spacy-4.0.0.dev0/spacy/matcher/levenshtein.pyx` & `spacy-4.0.0.dev1/spacy/matcher/levenshtein.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 cpdef bint levenshtein_compare(input_text: str, pattern_text: str, fuzzy: int = -1):
     if fuzzy >= 0:
         max_edits = fuzzy
     else:
         # allow at least two edits (to allow at least one transposition) and up
-        # to 20% of the pattern string length
+        # to 30% of the pattern string length
         max_edits = max(2, round(0.3 * len(pattern_text)))
     return levenshtein(input_text, pattern_text, max_edits) <= max_edits
 
 
 @registry.misc("spacy.levenshtein_compare.v1")
 def make_levenshtein_compare():
     return levenshtein_compare
```

### Comparing `spacy-4.0.0.dev0/spacy/matcher/matcher.pxd` & `spacy-4.0.0.dev1/spacy/matcher/matcher.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/matcher/matcher.pyi` & `spacy-4.0.0.dev1/spacy/matcher/matcher.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import Any, List, Dict, Tuple, Optional, Callable, Union
+from typing import Any, List, Dict, Tuple, Optional, Callable, Union, Literal
 from typing import Iterator, Iterable, overload
-from ..compat import Literal
 from ..vocab import Vocab
 from ..tokens import Doc, Span
 
 class Matcher:
-    def __init__(self, vocab: Vocab, validate: bool = ...,
-                 fuzzy_compare: Callable[[str, str, int], bool] = ...) -> None: ...
+    def __init__(
+        self,
+        vocab: Vocab,
+        validate: bool = ...,
+        fuzzy_compare: Callable[[str, str, int], bool] = ...,
+    ) -> None: ...
     def __reduce__(self) -> Any: ...
     def __len__(self) -> int: ...
     def __contains__(self, key: str) -> bool: ...
     def add(
         self,
         key: Union[str, int],
         patterns: List[List[Dict[str, Any]]],
```

### Comparing `spacy-4.0.0.dev0/spacy/matcher/matcher.pyx` & `spacy-4.0.0.dev1/spacy/matcher/matcher.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -825,14 +825,19 @@
             attr_values.append((attr, value))
         else:
             # should be caught in validation
             raise ValueError(Errors.E152.format(attr=input_attr))
     return attr_values
 
 
+def _predicate_cache_key(attr, predicate, value, *, regex=False, fuzzy=None):
+    # tuple order affects performance
+    return (attr, regex, fuzzy, predicate, srsly.json_dumps(value, sort_keys=True))
+
+
 # These predicate helper classes are used to match the REGEX, IN, >= etc
 # extensions to the matcher introduced in #3173.
 
 class _FuzzyPredicate:
     operators = ("FUZZY", "FUZZY1", "FUZZY2", "FUZZY3", "FUZZY4", "FUZZY5",
                  "FUZZY6", "FUZZY7", "FUZZY8", "FUZZY9")
 
@@ -844,15 +849,15 @@
         self.predicate = predicate
         self.is_extension = is_extension
         if self.predicate not in self.operators:
             raise ValueError(Errors.E126.format(good=self.operators, bad=self.predicate))
         fuzz = self.predicate[len("FUZZY"):] # number after prefix
         self.fuzzy = int(fuzz) if fuzz else -1
         self.fuzzy_compare = fuzzy_compare
-        self.key = (self.attr, self.fuzzy, self.predicate, srsly.json_dumps(value, sort_keys=True))
+        self.key = _predicate_cache_key(self.attr, self.predicate, value, fuzzy=self.fuzzy)
 
     def __call__(self, Token token):
         if self.is_extension:
             value = token._.get(self.attr)
         else:
             value = token.vocab.strings[get_token_attr_for_matcher(token.c, self.attr)]
         if self.value == value:
@@ -866,15 +871,15 @@
     def __init__(self, i, attr, value, predicate, is_extension=False, vocab=None,
                  regex=False, fuzzy=None, fuzzy_compare=None):
         self.i = i
         self.attr = attr
         self.value = re.compile(value)
         self.predicate = predicate
         self.is_extension = is_extension
-        self.key = (self.attr, self.predicate, srsly.json_dumps(value, sort_keys=True))
+        self.key = _predicate_cache_key(self.attr, self.predicate, value)
         if self.predicate not in self.operators:
             raise ValueError(Errors.E126.format(good=self.operators, bad=self.predicate))
 
     def __call__(self, Token token):
         if self.is_extension:
             value = token._.get(self.attr)
         else:
@@ -902,15 +907,15 @@
             elif self.fuzzy is not None:
                 # add to string store
                 self.value = set(self.vocab.strings.add(v) for v in value)
             else:
                 self.value = set(get_string_id(v) for v in value)
         self.predicate = predicate
         self.is_extension = is_extension
-        self.key = (self.attr, self.regex, self.fuzzy, self.predicate, srsly.json_dumps(value, sort_keys=True))
+        self.key = _predicate_cache_key(self.attr, self.predicate, value, regex=self.regex, fuzzy=self.fuzzy)
         if self.predicate not in self.operators:
             raise ValueError(Errors.E126.format(good=self.operators, bad=self.predicate))
 
     def __call__(self, Token token):
         if self.is_extension:
             value = token._.get(self.attr)
         else:
@@ -974,15 +979,15 @@
     def __init__(self, i, attr, value, predicate, is_extension=False, vocab=None,
                  regex=False, fuzzy=None, fuzzy_compare=None):
         self.i = i
         self.attr = attr
         self.value = value
         self.predicate = predicate
         self.is_extension = is_extension
-        self.key = (self.attr, self.predicate, srsly.json_dumps(value, sort_keys=True))
+        self.key = _predicate_cache_key(self.attr, self.predicate, value)
         if self.predicate not in self.operators:
             raise ValueError(Errors.E126.format(good=self.operators, bad=self.predicate))
 
     def __call__(self, Token token):
         if self.is_extension:
             value = token._.get(self.attr)
         else:
@@ -1089,15 +1094,15 @@
 def _get_extension_extra_predicates(spec, extra_predicates, predicate_types,
         seen_predicates):
     output = []
     for attr, value in spec.items():
         if isinstance(value, dict):
             for type_, cls in predicate_types.items():
                 if type_ in value:
-                    key = (attr, type_, srsly.json_dumps(value[type_], sort_keys=True))
+                    key = _predicate_cache_key(attr, type_, value[type_])
                     if key in seen_predicates:
                         output.append(seen_predicates[key])
                     else:
                         predicate = cls(len(extra_predicates), attr, value[type_], type_,
                                         is_extension=True)
                         extra_predicates.append(predicate)
                         output.append(predicate.i)
```

### Comparing `spacy-4.0.0.dev0/spacy/matcher/phrasematcher.pxd` & `spacy-4.0.0.dev1/spacy/matcher/phrasematcher.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/matcher/phrasematcher.pyi` & `spacy-4.0.0.dev1/spacy/matcher/phrasematcher.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import List, Tuple, Union, Optional, Callable, Any, Dict, overload
-from ..compat import Literal
+from typing import List, Tuple, Union, Optional, Callable, Any, Dict, Literal
+from typing import overload
 from .matcher import Matcher
 from ..vocab import Vocab
 from ..tokens import Doc, Span
 
 class PhraseMatcher:
     def __init__(
         self, vocab: Vocab, attr: Optional[Union[int, str]], validate: bool = ...
```

### Comparing `spacy-4.0.0.dev0/spacy/matcher/phrasematcher.pyx` & `spacy-4.0.0.dev1/spacy/matcher/phrasematcher.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/matcher/polyleven.c` & `spacy-4.0.0.dev1/spacy/matcher/polyleven.c`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/callbacks.py` & `spacy-4.0.0.dev1/spacy/ml/callbacks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/character_embed.py` & `spacy-4.0.0.dev1/spacy/ml/character_embed.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/extract_ngrams.py` & `spacy-4.0.0.dev1/spacy/ml/extract_ngrams.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/extract_spans.py` & `spacy-4.0.0.dev1/spacy/ml/extract_spans.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Callable
+from typing import List, Tuple, Callable
 from thinc.api import Model, to_numpy
 from thinc.types import Ragged, Ints1d
 
 from ..util import registry
 
 
 @registry.layers("spacy.extract_spans.v1")
@@ -48,19 +48,19 @@
 
 def _get_span_indices(ops, spans: Ragged, lengths: Ints1d) -> Ints1d:
     """Construct a flat array that has the indices we want to extract from the
     source data. For instance, if we want the spans (5, 9), (8, 10) the
     indices will be [5, 6, 7, 8, 8, 9].
     """
     spans, lengths = _ensure_cpu(spans, lengths)
-    indices = []
+    indices: List[int] = []
     offset = 0
     for i, length in enumerate(lengths):
         spans_i = spans[i].dataXd + offset
         for j in range(spans_i.shape[0]):
-            indices.append(ops.xp.arange(spans_i[j, 0], spans_i[j, 1]))  # type: ignore[call-overload, index]
+            indices.extend(range(spans_i[j, 0], spans_i[j, 1]))  # type: ignore[arg-type, call-overload]
         offset += length
-    return ops.flatten(indices, dtype="i", ndim_if_empty=1)
+    return ops.asarray1i(indices)
 
 
 def _ensure_cpu(spans: Ragged, lengths: Ints1d) -> Tuple[Ragged, Ints1d]:
     return Ragged(to_numpy(spans.dataXd), to_numpy(spans.lengths)), to_numpy(lengths)
```

### Comparing `spacy-4.0.0.dev0/spacy/ml/featureextractor.py` & `spacy-4.0.0.dev1/spacy/ml/featureextractor.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/entity_linker.py` & `spacy-4.0.0.dev1/spacy/ml/models/entity_linker.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import Optional, Callable, Iterable, List, Tuple
 from thinc.types import Floats2d
 from thinc.api import chain, list2ragged, reduce_mean, residual
 from thinc.api import Model, Maxout, Linear, tuplify, Ragged
 
 from ...util import registry
 from ...kb import KnowledgeBase, InMemoryLookupKB
-from ...kb import Candidate, get_candidates, get_candidates_batch
+from ...kb import Candidate
 from ...vocab import Vocab
-from ...tokens import Span, Doc
+from ...tokens import Doc, Span, SpanGroup
 from ..extract_spans import extract_spans
 from ...errors import Errors
 
 
 @registry.architectures("spacy.EntityLinker.v2")
 def build_nel_encoder(
     tok2vec: Model, nO: Optional[int] = None
@@ -85,14 +85,22 @@
         kb = InMemoryLookupKB(vocab, entity_vector_length=1)
         kb.from_disk(kb_path)
         return kb
 
     return kb_from_file
 
 
+@registry.misc("spacy.EmptyKB.v2")
+def empty_kb_for_config() -> Callable[[Vocab, int], KnowledgeBase]:
+    def empty_kb_factory(vocab: Vocab, entity_vector_length: int):
+        return InMemoryLookupKB(vocab=vocab, entity_vector_length=entity_vector_length)
+
+    return empty_kb_factory
+
+
 @registry.misc("spacy.EmptyKB.v1")
 def empty_kb(
     entity_vector_length: int,
 ) -> Callable[[Vocab], KnowledgeBase]:
     def empty_kb_factory(vocab: Vocab):
         return InMemoryLookupKB(vocab=vocab, entity_vector_length=entity_vector_length)
 
@@ -102,10 +110,32 @@
 @registry.misc("spacy.CandidateGenerator.v1")
 def create_candidates() -> Callable[[KnowledgeBase, Span], Iterable[Candidate]]:
     return get_candidates
 
 
 @registry.misc("spacy.CandidateBatchGenerator.v1")
 def create_candidates_batch() -> Callable[
-    [KnowledgeBase, Iterable[Span]], Iterable[Iterable[Candidate]]
+    [KnowledgeBase, SpanGroup], Iterable[Iterable[Candidate]]
 ]:
     return get_candidates_batch
+
+
+def get_candidates(kb: KnowledgeBase, mention: Span) -> Iterable[Candidate]:
+    """
+    Return candidate entities for a given mention and fetching appropriate entries from the index.
+    kb (KnowledgeBase): Knowledge base to query.
+    mention (Span): Entity mention for which to identify candidates.
+    RETURNS (Iterable[Candidate]): Identified candidates.
+    """
+    return kb.get_candidates(mention)
+
+
+def get_candidates_batch(
+    kb: KnowledgeBase, mentions: SpanGroup
+) -> Iterable[Iterable[Candidate]]:
+    """
+    Return candidate entities for the given mentions and fetching appropriate entries from the index.
+    kb (KnowledgeBase): Knowledge base to query.
+    mentions (SpanGroup): Entity mentions for which to identify candidates.
+    RETURNS (Iterable[Iterable[Candidate]]): Identified candidates.
+    """
+    return kb.get_candidates_batch(mentions)
```

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/multi_task.py` & `spacy-4.0.0.dev1/spacy/ml/models/multi_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Any, Optional, Iterable, Tuple, List, Callable, TYPE_CHECKING, cast
-from thinc.types import Floats2d
+from thinc.types import Floats2d, Ints1d
 from thinc.api import chain, Maxout, LayerNorm, Softmax, Linear, zero_init, Model
 from thinc.api import MultiSoftmax, list2array
 from thinc.api import to_categorical, CosineDistance, L2Distance
 from thinc.loss import Loss
 
 from ...util import registry, OOV_RANK
 from ...errors import Errors
-from ...attrs import ID
+from ...attrs import ID, ORTH
+from ...vectors import Mode as VectorsMode
 
 import numpy
 from functools import partial
 
 if TYPE_CHECKING:
     # This lets us add type hints for mypy etc. without causing circular imports
     from ...vocab import Vocab  # noqa: F401
@@ -63,22 +64,31 @@
     return create_characters_objective
 
 
 def get_vectors_loss(ops, docs, prediction, distance):
     """Compute a loss based on a distance between the documents' vectors and
     the prediction.
     """
-    # The simplest way to implement this would be to vstack the
-    # token.vector values, but that's a bit inefficient, especially on GPU.
-    # Instead we fetch the index into the vectors table for each of our tokens,
-    # and look them up all at once. This prevents data copying.
-    ids = ops.flatten([doc.to_array(ID).ravel() for doc in docs])
-    target = docs[0].vocab.vectors.data[ids]
-    target[ids == OOV_RANK] = 0
-    d_target, loss = distance(prediction, target)
+    vocab = docs[0].vocab
+    if vocab.vectors.mode == VectorsMode.default:
+        # The simplest way to implement this would be to vstack the
+        # token.vector values, but that's a bit inefficient, especially on GPU.
+        # Instead we fetch the index into the vectors table for each of our
+        # tokens, and look them up all at once. This prevents data copying.
+        ids = ops.flatten([doc.to_array(ID).ravel() for doc in docs])
+        target = docs[0].vocab.vectors.data[ids]
+        target[ids == OOV_RANK] = 0
+        d_target, loss = distance(prediction, target)
+    elif vocab.vectors.mode == VectorsMode.floret:
+        keys = ops.flatten([cast(Ints1d, doc.to_array(ORTH)) for doc in docs])
+        target = vocab.vectors.get_batch(keys)
+        target = ops.as_contig(target)
+        d_target, loss = distance(prediction, target)
+    else:
+        raise ValueError(Errors.E850.format(mode=vocab.vectors.mode))
     return loss, d_target
 
 
 def get_characters_loss(ops, docs, prediction, nr_char):
     """Compute a loss based on a number of characters predicted from the docs."""
     target_ids = numpy.vstack([doc.to_utf8_array(nr_char=nr_char) for doc in docs])
     target_ids = target_ids.reshape((-1,))
```

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/parser.py` & `spacy-4.0.0.dev1/spacy/ml/models/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from typing import Optional, List, Tuple, Any
+from typing import Optional, List, Tuple, Any, Literal
 from thinc.types import Floats2d
 from thinc.api import Model
 import warnings
 
 from ...errors import Errors, Warnings
-from ...compat import Literal
 from ...util import registry
 from ..tb_framework import TransitionModel
 from ...tokens.doc import Doc
 
 TransitionSystem = Any  # TODO
 State = Any  # TODO
```

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/spancat.py` & `spacy-4.0.0.dev1/spacy/ml/models/spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/tagger.py` & `spacy-4.0.0.dev1/spacy/ml/models/tagger.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/textcat.py` & `spacy-4.0.0.dev1/spacy/ml/models/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/models/tok2vec.py` & `spacy-4.0.0.dev1/spacy/ml/models/tok2vec.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/staticvectors.py` & `spacy-4.0.0.dev1/spacy/ml/staticvectors.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/ml/tb_framework.pyx` & `spacy-4.0.0.dev1/spacy/ml/tb_framework.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -245,17 +245,19 @@
     cdef int i, j
     cdef vector[StateC *] unfinished
     cdef ActivationsC activations = _alloc_activations(sizes)
     cdef np.ndarray step_scores
     cdef np.ndarray step_actions
 
     scores = []
-    while sizes.states >= 1:
+    while sizes.states >= 1 and (actions is None or len(actions) > 0):
         step_scores = numpy.empty((sizes.states, sizes.classes), dtype="f")
         step_actions = actions[0] if actions is not None else None
+        assert step_actions is None or step_actions.size == sizes.states, \
+            f"number of step actions ({step_actions.size}) must equal number of states ({sizes.states})"
         with nogil:
             _predict_states(cblas, &activations, <float*>step_scores.data, states, &weights, sizes)
             if actions is None:
                 # Validate actions, argmax, take action.
                 c_transition_batch(moves, states, <const float*>step_scores.data, sizes.classes,
                     sizes.states)
             else:
```

### Comparing `spacy-4.0.0.dev0/spacy/morphology.pxd` & `spacy-4.0.0.dev1/spacy/morphology.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/morphology.pyx` & `spacy-4.0.0.dev1/spacy/morphology.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/parts_of_speech.pxd` & `spacy-4.0.0.dev1/spacy/parts_of_speech.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipe_analysis.py` & `spacy-4.0.0.dev1/spacy/pipe_analysis.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/__init__.py` & `spacy-4.0.0.dev1/spacy/pipeline/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from .attribute_ruler import AttributeRuler
 from .dep_parser import DependencyParser
 from .edit_tree_lemmatizer import EditTreeLemmatizer
 from .entity_linker import EntityLinker
-from .ner import EntityRecognizer
+from .functions import merge_entities, merge_noun_chunks, merge_subtokens
 from .lemmatizer import Lemmatizer
 from .morphologizer import Morphologizer
+from .ner import EntityRecognizer
 from .pipe import Pipe
-from .trainable_pipe import TrainablePipe
-from .senter import SentenceRecognizer
 from .sentencizer import Sentencizer
+from .senter import SentenceRecognizer
+from .span_finder import SpanFinder
+from .span_ruler import SpanRuler
+from .spancat import SpanCategorizer
 from .tagger import Tagger
 from .textcat import TextCategorizer
-from .spancat import SpanCategorizer
-from .span_ruler import SpanRuler
 from .textcat_multilabel import MultiLabel_TextCategorizer
 from .tok2vec import Tok2Vec
-from .functions import merge_entities, merge_noun_chunks, merge_subtokens
+from .trainable_pipe import TrainablePipe
 
 __all__ = [
     "AttributeRuler",
     "DependencyParser",
     "EntityLinker",
     "EntityRecognizer",
     "Morphologizer",
     "Lemmatizer",
     "MultiLabel_TextCategorizer",
     "Pipe",
     "SentenceRecognizer",
     "Sentencizer",
     "SpanCategorizer",
+    "SpanFinder",
     "SpanRuler",
     "Tagger",
     "TextCategorizer",
     "Tok2Vec",
     "TrainablePipe",
     "merge_entities",
     "merge_noun_chunks",
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/edit_trees.pxd` & `spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/edit_trees.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/edit_trees.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/edit_trees.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_edit_tree_internals/schemas.py` & `spacy-4.0.0.dev1/spacy/pipeline/_edit_tree_internals/schemas.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_beam_utils.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_beam_utils.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_parser_utils.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_parser_utils.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/_state.pxd` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/_state.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/arc_eager.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/arc_eager.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/batch.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/batch.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/ner.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/ner.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/nonproj.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/nonproj.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/search.pxd` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/search.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/search.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/search.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/stateclass.pxd` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/stateclass.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/stateclass.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/stateclass.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/transition_system.pxd` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/transition_system.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/_parser_internals/transition_system.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/_parser_internals/transition_system.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/attribute_ruler.py` & `spacy-4.0.0.dev1/spacy/pipeline/attribute_ruler.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/dep_parser.py` & `spacy-4.0.0.dev1/spacy/pipeline/dep_parser.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/edit_tree_lemmatizer.py` & `spacy-4.0.0.dev1/spacy/pipeline/edit_tree_lemmatizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import cast, Any, Callable, Dict, Iterable, List, Optional, Union
 from typing import Tuple
 from collections import Counter
 from itertools import islice
 import numpy as np
 
 import srsly
-from thinc.api import Config, Model
+from thinc.api import Config, Model, SequenceCategoricalCrossentropy, NumpyOps
 from thinc.types import ArrayXd, Floats2d, Ints1d
 from thinc.legacy import LegacySequenceCategoricalCrossentropy
 
 from ._edit_tree_internals.edit_trees import EditTrees
 from ._edit_tree_internals.schemas import validate_edit_tree
 from .lemmatizer import lemmatizer_score
 from .trainable_pipe import TrainablePipe
@@ -18,14 +18,16 @@
 from ..tokens import Doc
 from ..training import Example, validate_examples, validate_get_examples
 from ..vocab import Vocab
 from .. import util
 
 
 ActivationsT = Dict[str, Union[List[Floats2d], List[Ints1d]]]
+# The cutoff value of *top_k* above which an alternative method is used to process guesses.
+TOP_K_GUARDRAIL = 20
 
 
 default_model_config = """
 [model]
 @architectures = "spacy.Tagger.v2"
 
 [model.tok2vec]
@@ -121,14 +123,15 @@
 
         self.trees = EditTrees(self.vocab.strings)
         self.tree2label: Dict[int, int] = {}
 
         self.cfg: Dict[str, Any] = {"labels": []}
         self.scorer = scorer
         self.save_activations = save_activations
+        self.numpy_ops = NumpyOps()
 
     def get_loss(
         self, examples: Iterable[Example], scores: List[Floats2d]
     ) -> Tuple[float, List[Floats2d]]:
         validate_examples(examples, "EditTreeLemmatizer.get_loss")
         loss_func = LegacySequenceCategoricalCrossentropy(
             normalize=False, missing_value=-1
@@ -136,15 +139,15 @@
 
         truths = []
         for eg in examples:
             eg_truths = []
             for (predicted, gold_lemma) in zip(
                 eg.predicted, eg.get_aligned("LEMMA", as_string=True)
             ):
-                if gold_lemma is None:
+                if gold_lemma is None or gold_lemma == "":
                     label = -1
                 else:
                     tree_id = self.trees.add(predicted.text, gold_lemma)
                     label = self.tree2label.get(tree_id, 0)
                 eg_truths.append(label)
 
             truths.append(eg_truths)
@@ -161,52 +164,96 @@
         """Calculate the loss and its gradient for a batch of student
         scores, relative to teacher scores.
 
         teacher_scores: Scores representing the teacher model's predictions.
         student_scores: Scores representing the student model's predictions.
 
         RETURNS (Tuple[float, float]): The loss and the gradient.
-        
+
         DOCS: https://spacy.io/api/edittreelemmatizer#get_teacher_student_loss
         """
         loss_func = LegacySequenceCategoricalCrossentropy(normalize=False)
         d_scores, loss = loss_func(student_scores, teacher_scores)
         if self.model.ops.xp.isnan(loss):
             raise ValueError(Errors.E910.format(name=self.name))
         return float(loss), d_scores
 
     def predict(self, docs: Iterable[Doc]) -> ActivationsT:
+        if self.top_k == 1:
+            scores2guesses = self._scores2guesses_top_k_equals_1
+        elif self.top_k <= TOP_K_GUARDRAIL:
+            scores2guesses = self._scores2guesses_top_k_greater_1
+        else:
+            scores2guesses = self._scores2guesses_top_k_guardrail
+        # The behaviour of *_scores2guesses_top_k_greater_1()* is efficient for values
+        # of *top_k>1* that are likely to be useful when the edit tree lemmatizer is used
+        # for its principal purpose of lemmatizing tokens. However, the code could also
+        # be used for other purposes, and with very large values of *top_k* the method
+        # becomes inefficient. In such cases, *_scores2guesses_top_k_guardrail()* is used
+        # instead.
         n_docs = len(list(docs))
         if not any(len(doc) for doc in docs):
             # Handle cases where there are no tokens in any docs.
             n_labels = len(self.cfg["labels"])
             guesses: List[Ints1d] = [
                 self.model.ops.alloc((0,), dtype="i") for doc in docs
             ]
             scores: List[Floats2d] = [
                 self.model.ops.alloc((0, n_labels), dtype="i") for doc in docs
             ]
             assert len(guesses) == n_docs
             return {"probabilities": scores, "tree_ids": guesses}
         scores = self.model.predict(docs)
         assert len(scores) == n_docs
-        guesses = self._scores2guesses(docs, scores)
+        guesses = scores2guesses(docs, scores)
         assert len(guesses) == n_docs
         return {"probabilities": scores, "tree_ids": guesses}
 
-    def _scores2guesses(self, docs, scores):
+    def _scores2guesses_top_k_equals_1(self, docs, scores):
+        guesses = []
+        for doc, doc_scores in zip(docs, scores):
+            doc_guesses = doc_scores.argmax(axis=1)
+            doc_guesses = self.numpy_ops.asarray(doc_guesses)
+
+            doc_compat_guesses = []
+            for i, token in enumerate(doc):
+                tree_id = self.cfg["labels"][doc_guesses[i]]
+                if self.trees.apply(tree_id, token.text) is not None:
+                    doc_compat_guesses.append(tree_id)
+                else:
+                    doc_compat_guesses.append(-1)
+            guesses.append(np.array(doc_compat_guesses))
+
+        return guesses
+
+    def _scores2guesses_top_k_greater_1(self, docs, scores):
         guesses = []
+        top_k = min(self.top_k, len(self.labels))
         for doc, doc_scores in zip(docs, scores):
-            if self.top_k == 1:
-                doc_guesses = doc_scores.argmax(axis=1).reshape(-1, 1)
-            else:
-                doc_guesses = np.argsort(doc_scores)[..., : -self.top_k - 1 : -1]
+            doc_scores = self.numpy_ops.asarray(doc_scores)
+            doc_compat_guesses = []
+            for i, token in enumerate(doc):
+                for _ in range(top_k):
+                    candidate = int(doc_scores[i].argmax())
+                    candidate_tree_id = self.cfg["labels"][candidate]
+                    if self.trees.apply(candidate_tree_id, token.text) is not None:
+                        doc_compat_guesses.append(candidate_tree_id)
+                        break
+                    doc_scores[i, candidate] = np.finfo(np.float32).min
+                else:
+                    doc_compat_guesses.append(-1)
+            guesses.append(np.array(doc_compat_guesses))
 
-            if not isinstance(doc_guesses, np.ndarray):
-                doc_guesses = doc_guesses.get()
+        return guesses
+
+    def _scores2guesses_top_k_guardrail(self, docs, scores):
+        guesses = []
+        for doc, doc_scores in zip(docs, scores):
+            doc_guesses = np.argsort(doc_scores)[..., : -self.top_k - 1 : -1]
+            doc_guesses = self.numpy_ops.asarray(doc_guesses)
 
             doc_compat_guesses = []
             for token, candidates in zip(doc, doc_guesses):
                 tree_id = -1
                 for candidate in candidates:
                     candidate_tree_id = self.cfg["labels"][candidate]
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/entity_linker.py` & `spacy-4.0.0.dev1/spacy/pipeline/entity_linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-from typing import Optional, Iterable, Callable, Dict, Sequence, Union, List, Any
-from typing import cast
+import warnings
+from typing import Optional, Iterable, Callable, Dict, Sequence, Union, List, Any, cast
 from numpy import dtype
 from thinc.types import Floats1d, Floats2d, Ints1d, Ragged
 from pathlib import Path
 from itertools import islice
 import srsly
 import random
 from thinc.api import CosineDistance, Model, Optimizer, Config
 from thinc.api import set_dropout_rate
 
 from ..kb import KnowledgeBase, Candidate
-from ..ml import empty_kb
 from ..tokens import Doc, Span
+from ..ml import empty_kb
+from ..tokens import Doc, Span, SpanGroup
 from .pipe import deserialize_config
-from .legacy.entity_linker import EntityLinker_v1
 from .trainable_pipe import TrainablePipe
 from ..language import Language
 from ..vocab import Vocab
 from ..training import Example, validate_examples, validate_get_examples
-from ..errors import Errors
+from ..errors import Errors, Warnings
 from ..util import SimpleFrozenList, registry
 from .. import util
 from ..scorer import Scorer
 
 
 ActivationsT = Dict[str, Union[List[Ragged], List[str]]]
 
 KNOWLEDGE_BASE_IDS = "kb_ids"
 
-# See #9050
-BACKWARD_OVERWRITE = True
-
 default_model_config = """
 [model]
 @architectures = "spacy.EntityLinker.v2"
 
 [model.tok2vec]
 @architectures = "spacy.HashEmbedCNN.v2"
 pretrained_vectors = null
@@ -57,15 +54,16 @@
         "labels_discard": [],
         "n_sents": 0,
         "incl_prior": True,
         "incl_context": True,
         "entity_vector_length": 64,
         "get_candidates": {"@misc": "spacy.CandidateGenerator.v1"},
         "get_candidates_batch": {"@misc": "spacy.CandidateBatchGenerator.v1"},
-        "overwrite": True,
+        "overwrite": False,
+        "generate_empty_kb": {"@misc": "spacy.EmptyKB.v2"},
         "scorer": {"@scorers": "spacy.entity_linker_scorer.v1"},
         "use_gold_ents": True,
         "candidates_batch_size": 1,
         "threshold": None,
         "save_activations": False,
     },
     default_score_weights={
@@ -82,16 +80,17 @@
     labels_discard: Iterable[str],
     n_sents: int,
     incl_prior: bool,
     incl_context: bool,
     entity_vector_length: int,
     get_candidates: Callable[[KnowledgeBase, Span], Iterable[Candidate]],
     get_candidates_batch: Callable[
-        [KnowledgeBase, Iterable[Span]], Iterable[Iterable[Candidate]]
+        [KnowledgeBase, SpanGroup], Iterable[Iterable[Candidate]]
     ],
+    generate_empty_kb: Callable[[Vocab, int], KnowledgeBase],
     overwrite: bool,
     scorer: Optional[Callable],
     use_gold_ents: bool,
     candidates_batch_size: int,
     threshold: Optional[float] = None,
     save_activations: bool,
 ):
@@ -104,51 +103,40 @@
     n_sents (int): The number of neighbouring sentences to take into account.
     incl_prior (bool): Whether or not to include prior probabilities from the KB in the model.
     incl_context (bool): Whether or not to include the local context in the model.
     entity_vector_length (int): Size of encoding vectors in the KB.
     get_candidates (Callable[[KnowledgeBase, Span], Iterable[Candidate]]): Function that
         produces a list of candidates, given a certain knowledge base and a textual mention.
     get_candidates_batch (
-        Callable[[KnowledgeBase, Iterable[Span]], Iterable[Iterable[Candidate]]], Iterable[Candidate]]
+        Callable[[KnowledgeBase, SpanGroup], Iterable[Iterable[Candidate]]], Iterable[Candidate]]
         ): Function that produces a list of candidates, given a certain knowledge base and several textual mentions.
+    generate_empty_kb (Callable[[Vocab, int], KnowledgeBase]): Callable returning empty KnowledgeBase.
     scorer (Optional[Callable]): The scoring method.
     use_gold_ents (bool): Whether to copy entities from gold docs or not. If false, another
         component must provide entity annotations.
     candidates_batch_size (int): Size of batches for entity candidate generation.
     threshold (Optional[float]): Confidence threshold for entity predictions. If confidence is below the threshold,
         prediction is discarded. If None, predictions are not filtered by any threshold.
     save_activations (bool): save model activations in Doc when annotating.
     """
-
     if not model.attrs.get("include_span_maker", False):
-        # The only difference in arguments here is that use_gold_ents and threshold aren't available.
-        return EntityLinker_v1(
-            nlp.vocab,
-            model,
-            name,
-            labels_discard=labels_discard,
-            n_sents=n_sents,
-            incl_prior=incl_prior,
-            incl_context=incl_context,
-            entity_vector_length=entity_vector_length,
-            get_candidates=get_candidates,
-            overwrite=overwrite,
-            scorer=scorer,
-        )
+        raise ValueError(Errors.E4005)
+
     return EntityLinker(
         nlp.vocab,
         model,
         name,
         labels_discard=labels_discard,
         n_sents=n_sents,
         incl_prior=incl_prior,
         incl_context=incl_context,
         entity_vector_length=entity_vector_length,
         get_candidates=get_candidates,
         get_candidates_batch=get_candidates_batch,
+        generate_empty_kb=generate_empty_kb,
         overwrite=overwrite,
         scorer=scorer,
         use_gold_ents=use_gold_ents,
         candidates_batch_size=candidates_batch_size,
         threshold=threshold,
         save_activations=save_activations,
     )
@@ -180,17 +168,18 @@
         labels_discard: Iterable[str],
         n_sents: int,
         incl_prior: bool,
         incl_context: bool,
         entity_vector_length: int,
         get_candidates: Callable[[KnowledgeBase, Span], Iterable[Candidate]],
         get_candidates_batch: Callable[
-            [KnowledgeBase, Iterable[Span]], Iterable[Iterable[Candidate]]
+            [KnowledgeBase, SpanGroup], Iterable[Iterable[Candidate]]
         ],
-        overwrite: bool = BACKWARD_OVERWRITE,
+        generate_empty_kb: Callable[[Vocab, int], KnowledgeBase],
+        overwrite: bool = False,
         scorer: Optional[Callable] = entity_linker_score,
         use_gold_ents: bool,
         candidates_batch_size: int,
         threshold: Optional[float] = None,
         save_activations: bool = False,
     ) -> None:
         """Initialize an entity linker.
@@ -203,23 +192,26 @@
         n_sents (int): The number of neighbouring sentences to take into account.
         incl_prior (bool): Whether or not to include prior probabilities from the KB in the model.
         incl_context (bool): Whether or not to include the local context in the model.
         entity_vector_length (int): Size of encoding vectors in the KB.
         get_candidates (Callable[[KnowledgeBase, Span], Iterable[Candidate]]): Function that
             produces a list of candidates, given a certain knowledge base and a textual mention.
         get_candidates_batch (
-            Callable[[KnowledgeBase, Iterable[Span]], Iterable[Iterable[Candidate]]],
+            Callable[[KnowledgeBase, SpanGroup], Iterable[Iterable[Candidate]]],
             Iterable[Candidate]]
             ): Function that produces a list of candidates, given a certain knowledge base and several textual mentions.
+        generate_empty_kb (Callable[[Vocab, int], KnowledgeBase]): Callable returning empty KnowledgeBase.
+        overwrite (bool): Whether to overwrite existing non-empty annotations.
         scorer (Optional[Callable]): The scoring method. Defaults to Scorer.score_links.
         use_gold_ents (bool): Whether to copy entities from gold docs or not. If false, another
             component must provide entity annotations.
         candidates_batch_size (int): Size of batches for entity candidate generation.
         threshold (Optional[float]): Confidence threshold for entity predictions. If confidence is below the
             threshold, prediction is discarded. If None, predictions are not filtered by any threshold.
+        save_activations (bool): save model activations in Doc when annotating.
         DOCS: https://spacy.io/api/entitylinker#init
         """
 
         if threshold is not None and not (0 <= threshold <= 1):
             raise ValueError(
                 Errors.E1043.format(
                     range_start=0,
@@ -228,46 +220,47 @@
                 )
             )
 
         self.vocab = vocab
         self.model = model
         self.name = name
         self.labels_discard = list(labels_discard)
+        # how many neighbour sentences to take into account
         self.n_sents = n_sents
         self.incl_prior = incl_prior
         self.incl_context = incl_context
         self.get_candidates = get_candidates
         self.get_candidates_batch = get_candidates_batch
         self.cfg: Dict[str, Any] = {"overwrite": overwrite}
         self.distance = CosineDistance(normalize=False)
-        # how many neighbour sentences to take into account
-        # create an empty KB by default
-        self.kb = empty_kb(entity_vector_length)(self.vocab)
+        self.kb = generate_empty_kb(self.vocab, entity_vector_length)
         self.scorer = scorer
         self.use_gold_ents = use_gold_ents
         self.candidates_batch_size = candidates_batch_size
         self.threshold = threshold
         self.save_activations = save_activations
 
         if candidates_batch_size < 1:
             raise ValueError(Errors.E1044)
+        if self.incl_prior and not self.kb.supports_prior_probs:
+            warnings.warn(Warnings.W401)
 
     def set_kb(self, kb_loader: Callable[[Vocab], KnowledgeBase]):
         """Define the KB of this pipe by providing a function that will
         create it using this object's vocab."""
         if not callable(kb_loader):
             raise ValueError(Errors.E885.format(arg_type=type(kb_loader)))
 
         self.kb = kb_loader(self.vocab)  # type: ignore
 
     def validate_kb(self) -> None:
         # Raise an error if the knowledge base is not initialized.
         if self.kb is None:
             raise ValueError(Errors.E1018.format(name=self.name))
-        if len(self.kb) == 0:
+        if hasattr(self.kb, "is_empty") and self.kb.is_empty():
             raise ValueError(Errors.E139.format(name=self.name))
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable[Example]],
         *,
         nlp: Optional[Language] = None,
@@ -449,15 +442,19 @@
         entity_count = 0
         final_kb_ids: List[str] = []
         ops = self.model.ops
         xp = ops.xp
         docs_ents: List[Ragged] = []
         docs_scores: List[Ragged] = []
         if not docs:
-            return {KNOWLEDGE_BASE_IDS: final_kb_ids, "ents": docs_ents, "scores": docs_scores}
+            return {
+                KNOWLEDGE_BASE_IDS: final_kb_ids,
+                "ents": docs_ents,
+                "scores": docs_scores,
+            }
         if isinstance(docs, Doc):
             docs = [docs]
         for doc in docs:
             doc_ents: List[Ints1d] = []
             doc_scores: List[Floats1d] = []
             if len(doc) == 0:
                 docs_scores.append(Ragged(ops.alloc1f(0), ops.alloc1i(0)))
@@ -474,37 +471,44 @@
                     idx
                     for idx in range(len(ent_batch))
                     if ent_batch[idx].label_ not in self.labels_discard
                 ]
 
                 batch_candidates = list(
                     self.get_candidates_batch(
-                        self.kb, [ent_batch[idx] for idx in valid_ent_idx]
+                        self.kb,
+                        SpanGroup(doc, spans=[ent_batch[idx] for idx in valid_ent_idx]),
                     )
                     if self.candidates_batch_size > 1
                     else [
                         self.get_candidates(self.kb, ent_batch[idx])
                         for idx in valid_ent_idx
                     ]
                 )
 
                 # Looping through each entity in batch (TODO: rewrite)
                 for j, ent in enumerate(ent_batch):
-                    sent_index = sentences.index(ent.sent)
-                    assert sent_index >= 0
+                    assert hasattr(ent, "sents")
+                    sents = list(ent.sents)
+                    sent_indices = (
+                        sentences.index(sents[0]),
+                        sentences.index(sents[-1]),
+                    )
+                    assert sent_indices[1] >= sent_indices[0] >= 0
 
                     if self.incl_context:
                         # get n_neighbour sentences, clipped to the length of the document
-                        start_sentence = max(0, sent_index - self.n_sents)
+                        start_sentence = max(0, sent_indices[0] - self.n_sents)
                         end_sentence = min(
-                            len(sentences) - 1, sent_index + self.n_sents
+                            len(sentences) - 1, sent_indices[1] + self.n_sents
                         )
                         start_token = sentences[start_sentence].start
                         end_token = sentences[end_sentence].end
                         sent_doc = doc[start_token:end_token].as_doc()
+
                         # currently, the context is the same for each entity in a sentence (should be refined)
                         sentence_encoding = self.model.predict([sent_doc])[0]
                         sentence_encoding_t = sentence_encoding.T
                         sentence_norm = xp.linalg.norm(sentence_encoding_t)
                     entity_count += 1
                     if ent.label_ in self.labels_discard:
                         # ignoring this entity - setting to NIL
@@ -524,26 +528,27 @@
                                 doc_scores=doc_scores,
                                 doc_ents=doc_ents,
                                 scores=[0.0],
                                 ents=[0],
                             )
                         elif len(candidates) == 1 and self.threshold is None:
                             # shortcut for efficiency reasons: take the 1 candidate
-                            final_kb_ids.append(candidates[0].entity_)
+                            final_kb_ids.append(candidates[0].entity_id_)
                             self._add_activations(
                                 doc_scores=doc_scores,
                                 doc_ents=doc_ents,
                                 scores=[1.0],
-                                ents=[candidates[0].entity_],
+                                ents=[candidates[0].entity_id],
                             )
                         else:
                             random.shuffle(candidates)
                             # set all prior probabilities to 0 if incl_prior=False
-                            prior_probs = xp.asarray([c.prior_prob for c in candidates])
-                            if not self.incl_prior:
+                            if self.incl_prior and self.kb.supports_prior_probs:
+                                prior_probs = xp.asarray([c.prior_prob for c in candidates])  # type: ignore
+                            else:
                                 prior_probs = xp.asarray([0.0 for _ in candidates])
                             scores = prior_probs
                             # add in similarity from the context
                             if self.incl_context:
                                 entity_encodings = xp.asarray(
                                     [c.entity_vector for c in candidates]
                                 )
@@ -559,37 +564,41 @@
                                 sims = xp.dot(entity_encodings, sentence_encoding_t) / (
                                     sentence_norm * entity_norm
                                 )
                                 if sims.shape != prior_probs.shape:
                                     raise ValueError(Errors.E161)
                                 scores = prior_probs + sims - (prior_probs * sims)
                             final_kb_ids.append(
-                                candidates[scores.argmax().item()].entity_
+                                candidates[scores.argmax().item()].entity_id_
                                 if self.threshold is None
                                 or scores.max() >= self.threshold
                                 else EntityLinker.NIL
                             )
                             self._add_activations(
                                 doc_scores=doc_scores,
                                 doc_ents=doc_ents,
                                 scores=scores,
-                                ents=[c.entity for c in candidates],
+                                ents=[c.entity_id for c in candidates],
                             )
             self._add_doc_activations(
                 docs_scores=docs_scores,
                 docs_ents=docs_ents,
                 doc_scores=doc_scores,
                 doc_ents=doc_ents,
             )
         if not (len(final_kb_ids) == entity_count):
             err = Errors.E147.format(
                 method="predict", msg="result variables not of equal length"
             )
             raise RuntimeError(err)
-        return {KNOWLEDGE_BASE_IDS: final_kb_ids, "ents": docs_ents, "scores": docs_scores}
+        return {
+            KNOWLEDGE_BASE_IDS: final_kb_ids,
+            "ents": docs_ents,
+            "scores": docs_scores,
+        }
 
     def set_annotations(self, docs: Iterable[Doc], activations: ActivationsT) -> None:
         """Modify a batch of documents, using pre-computed scores.
 
         docs (Iterable[Doc]): The documents to modify.
         activations (ActivationsT): The activations used for setting annotations, produced
                                  by EntityLinker.predict.
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/functions.py` & `spacy-4.0.0.dev1/spacy/pipeline/functions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/lemmatizer.py` & `spacy-4.0.0.dev1/spacy/pipeline/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/morphologizer.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/morphologizer.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -55,28 +55,30 @@
     "morphologizer",
     assigns=["token.morph", "token.pos"],
     default_config={
         "model": DEFAULT_MORPH_MODEL,
         "overwrite": True,
         "extend": False,
         "scorer": {"@scorers": "spacy.morphologizer_scorer.v1"},
+        "label_smoothing": 0.0,
         "save_activations": False,
     },
     default_score_weights={"pos_acc": 0.5, "morph_acc": 0.5, "morph_per_feat": None},
 )
 def make_morphologizer(
     nlp: Language,
     model: Model,
     name: str,
     overwrite: bool,
     extend: bool,
+    label_smoothing: float,
     scorer: Optional[Callable],
     save_activations: bool,
 ):
-    return Morphologizer(nlp.vocab, model, name, overwrite=overwrite, extend=extend, scorer=scorer,
+    return Morphologizer(nlp.vocab, model, name, overwrite=overwrite, extend=extend, label_smoothing=label_smoothing, scorer=scorer,
                          save_activations=save_activations)
 
 
 def morphologizer_score(examples, **kwargs):
     def morph_key_getter(token, attr):
         return getattr(token, attr).key
 
@@ -100,23 +102,26 @@
         self,
         vocab: Vocab,
         model: Model,
         name: str = "morphologizer",
         *,
         overwrite: bool = BACKWARD_OVERWRITE,
         extend: bool = BACKWARD_EXTEND,
+        label_smoothing: float = 0.0,
         scorer: Optional[Callable] = morphologizer_score,
         save_activations: bool = False,
     ):
         """Initialize a morphologizer.
 
         vocab (Vocab): The shared vocabulary.
         model (thinc.api.Model): The Thinc Model powering the pipeline component.
         name (str): The component instance name, used to add entries to the
             losses during training.
+        overwrite (bool): Whether to overwrite existing annotations.
+        extend (bool): Whether to extend existing annotations.
         scorer (Optional[Callable]): The scoring method. Defaults to
             Scorer.score_token_attr for the attributes "pos" and "morph" and
             Scorer.score_token_attr_per_feat for the attribute "morph".
         save_activations (bool): save model activations in Doc when annotating.
 
         DOCS: https://spacy.io/api/morphologizer#init
         """
@@ -129,23 +134,24 @@
         # 1) labels_morph stores a mapping from morph+POS->morph
         # 2) labels_pos stores a mapping from morph+POS->POS
         cfg = {
             "labels_morph": {},
             "labels_pos": {},
             "overwrite": overwrite,
             "extend": extend,
+            "label_smoothing": label_smoothing,
         }
         self.cfg = dict(sorted(cfg.items()))
         self.scorer = scorer
         self.save_activations = save_activations
 
     @property
     def labels(self):
         """RETURNS (Iterable[str]): The labels currently added to the component."""
-        return self.cfg["labels_morph"].keys()
+        return tuple(self.cfg["labels_morph"].keys())
 
     @property
     def label_data(self) -> Dict[str, Dict[str, Union[str, float, int, None]]]:
         """A dictionary with all labels data."""
         return {"morph": self.cfg["labels_morph"], "pos": self.cfg["labels_pos"]}
 
     def add_label(self, label):
@@ -287,15 +293,16 @@
         examples (Iterable[Examples]): The batch of examples.
         scores: Scores representing the model's predictions.
         RETURNS (Tuple[float, float]): The loss and the gradient.
 
         DOCS: https://spacy.io/api/morphologizer#get_loss
         """
         validate_examples(examples, "Morphologizer.get_loss")
-        loss_func = LegacySequenceCategoricalCrossentropy(names=tuple(self.labels), normalize=False)
+        loss_func = LegacySequenceCategoricalCrossentropy(names=self.labels, normalize=False,
+                                                          label_smoothing=self.cfg["label_smoothing"])
         truths = []
         for eg in examples:
             eg_truths = []
             pos_tags = eg.get_aligned("POS", as_string=True)
             morphs = eg.get_aligned("MORPH", as_string=True)
             for i in range(len(morphs)):
                 pos = pos_tags[i]
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/ner.py` & `spacy-4.0.0.dev1/spacy/pipeline/ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,19 @@
                 labeller.model.get_ref("output_layer").set_dim("nO", len(self.labels))
             labeller.initialize(get_examples, nlp=nlp)
 
     @property
     def labels(self):
         # Get the labels from the model by looking at the available moves, e.g.
         # B-PERSON, I-PERSON, L-PERSON, U-PERSON
-        labels = set(remove_bilu_prefix(move) for move in self.move_names
-                     if move[0] in ("B", "I", "L", "U"))
+        labels = set(
+            remove_bilu_prefix(move)
+            for move in self.move_names
+            if move[0] in ("B", "I", "L", "U")
+        )
         return tuple(sorted(labels))
 
     def scored_ents(self, beams):
         """Return a dictionary of (start, end, label) tuples with corresponding scores
         for each beam/doc that was processed.
         """
         entity_scores = []
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/pipe.pyi` & `spacy-4.0.0.dev1/spacy/pipeline/pipe.pyi`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/pipe.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/pipe.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/sentencizer.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/sentencizer.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 
 from .pipe import Pipe
 from .senter import senter_score
 from ..language import Language
 from ..scorer import Scorer
 from .. import util
 
-# see #9050
-BACKWARD_OVERWRITE = False
-
 @Language.factory(
     "sentencizer",
     assigns=["token.is_sent_start", "doc.sents"],
     default_config={"punct_chars": None, "overwrite": False, "scorer": {"@scorers": "spacy.senter_scorer.v1"}},
     default_score_weights={"sents_f": 1.0, "sents_p": 0.0, "sents_r": 0.0},
 )
 def make_sentencizer(
@@ -48,21 +45,22 @@
             '｡', '。']
 
     def __init__(
         self,
         name="sentencizer",
         *,
         punct_chars=None,
-        overwrite=BACKWARD_OVERWRITE,
+        overwrite=False,
         scorer=senter_score,
     ):
         """Initialize the sentencizer.
 
         punct_chars (list): Punctuation characters to split on. Will be
             serialized with the nlp object.
+        overwrite (bool): Whether to overwrite existing annotations.
         scorer (Optional[Callable]): The scoring method. Defaults to
             Scorer.score_spans for the attribute "sents".
 
         DOCS: https://spacy.io/api/sentencizer#init
         """
         self.name = name
         if punct_chars:
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/senter.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/senter.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 from ..language import Language
 from ..errors import Errors
 from ..scorer import Scorer
 from ..training import validate_examples, validate_get_examples
 from ..util import registry
 from .. import util
 
-# See #9050
-BACKWARD_OVERWRITE = False
 
 default_model_config = """
 [model]
 @architectures = "spacy.Tagger.v2"
 
 [model.tok2vec]
 @architectures = "spacy.HashEmbedCNN.v2"
@@ -79,24 +77,25 @@
     """
     def __init__(
         self,
         vocab,
         model,
         name="senter",
         *,
-        overwrite=BACKWARD_OVERWRITE,
+        overwrite=False,
         scorer=senter_score,
         save_activations: bool = False,
     ):
         """Initialize a sentence recognizer.
 
         vocab (Vocab): The shared vocabulary.
         model (thinc.api.Model): The Thinc Model powering the pipeline component.
         name (str): The component instance name, used to add entries to the
             losses during training.
+        overwrite (bool): Whether to overwrite existing annotations.
         scorer (Optional[Callable]): The scoring method. Defaults to
             Scorer.score_spans for the attribute "sents".
         save_activations (bool): save model activations in Doc when annotating.
 
         DOCS: https://spacy.io/api/sentencerecognizer#init
         """
         self.vocab = vocab
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/span_ruler.py` & `spacy-4.0.0.dev1/spacy/pipeline/span_ruler.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/spancat.py` & `spacy-4.0.0.dev1/spacy/pipeline/trainable_pipe.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -1,502 +1,421 @@
-from typing import List, Dict, Callable, Tuple, Optional, Iterable, Any, cast
-from typing import Union
-from thinc.api import Config, Model, get_current_ops, set_dropout_rate, Ops
-from thinc.api import Optimizer
-from thinc.types import Ragged, Ints2d, Floats2d
-
-import numpy
-
-from ..compat import Protocol, runtime_checkable
-from ..scorer import Scorer
-from ..language import Language
-from .trainable_pipe import TrainablePipe
-from ..tokens import Doc, SpanGroup, Span
+# cython: infer_types=True, profile=True, binding=True
+from typing import Iterable, Iterator, Optional, Dict, Tuple, Callable
+import srsly
+from thinc.api import set_dropout_rate, Model, Optimizer
+import warnings
+
+from ..tokens.doc cimport Doc
+
+from ..training import validate_examples, validate_distillation_examples
+from ..errors import Errors, Warnings
+from .pipe import Pipe, deserialize_config
+from .. import util
 from ..vocab import Vocab
-from ..training import Example, validate_examples
-from ..errors import Errors
-from ..util import registry
-
-
-ActivationsT = Dict[str, Union[Floats2d, Ragged]]
-
-
-spancat_default_config = """
-[model]
-@architectures = "spacy.SpanCategorizer.v1"
-scorer = {"@layers": "spacy.LinearLogistic.v1"}
-
-[model.reducer]
-@layers = spacy.mean_max_reducer.v1
-hidden_size = 128
-
-[model.tok2vec]
-@architectures = "spacy.Tok2Vec.v2"
-
-[model.tok2vec.embed]
-@architectures = "spacy.MultiHashEmbed.v2"
-width = 96
-rows = [5000, 2000, 1000, 1000]
-attrs = ["ORTH", "PREFIX", "SUFFIX", "SHAPE"]
-include_static_vectors = false
-
-[model.tok2vec.encode]
-@architectures = "spacy.MaxoutWindowEncoder.v2"
-width = ${model.tok2vec.embed.width}
-window_size = 1
-maxout_pieces = 3
-depth = 4
-"""
-
-DEFAULT_SPANCAT_MODEL = Config().from_str(spancat_default_config)["model"]
-
-
-@runtime_checkable
-class Suggester(Protocol):
-    def __call__(self, docs: Iterable[Doc], *, ops: Optional[Ops] = None) -> Ragged:
-        ...
-
-
-@registry.misc("spacy.ngram_suggester.v1")
-def build_ngram_suggester(sizes: List[int]) -> Suggester:
-    """Suggest all spans of the given lengths. Spans are returned as a ragged
-    array of integers. The array has two columns, indicating the start and end
-    position."""
-
-    def ngram_suggester(docs: Iterable[Doc], *, ops: Optional[Ops] = None) -> Ragged:
-        if ops is None:
-            ops = get_current_ops()
-        spans = []
-        lengths = []
-        for doc in docs:
-            starts = ops.xp.arange(len(doc), dtype="i")
-            starts = starts.reshape((-1, 1))
-            length = 0
-            for size in sizes:
-                if size <= len(doc):
-                    starts_size = starts[: len(doc) - (size - 1)]
-                    spans.append(ops.xp.hstack((starts_size, starts_size + size)))
-                    length += spans[-1].shape[0]
-                if spans:
-                    assert spans[-1].ndim == 2, spans[-1].shape
-            lengths.append(length)
-        lengths_array = ops.asarray1i(lengths)
-        if len(spans) > 0:
-            output = Ragged(ops.xp.vstack(spans), lengths_array)
-        else:
-            output = Ragged(ops.xp.zeros((0, 0), dtype="i"), lengths_array)
-
-        assert output.dataXd.ndim == 2
-        return output
-
-    return ngram_suggester
-
-
-@registry.misc("spacy.ngram_range_suggester.v1")
-def build_ngram_range_suggester(min_size: int, max_size: int) -> Suggester:
-    """Suggest all spans of the given lengths between a given min and max value - both inclusive.
-    Spans are returned as a ragged array of integers. The array has two columns,
-    indicating the start and end position."""
-    sizes = list(range(min_size, max_size + 1))
-    return build_ngram_suggester(sizes)
-
-
-@Language.factory(
-    "spancat",
-    assigns=["doc.spans"],
-    default_config={
-        "threshold": 0.5,
-        "spans_key": "sc",
-        "max_positive": None,
-        "model": DEFAULT_SPANCAT_MODEL,
-        "suggester": {"@misc": "spacy.ngram_suggester.v1", "sizes": [1, 2, 3]},
-        "scorer": {"@scorers": "spacy.spancat_scorer.v1"},
-        "save_activations": False,
-    },
-    default_score_weights={"spans_sc_f": 1.0, "spans_sc_p": 0.0, "spans_sc_r": 0.0},
-)
-def make_spancat(
-    nlp: Language,
-    name: str,
-    suggester: Suggester,
-    model: Model[Tuple[List[Doc], Ragged], Floats2d],
-    spans_key: str,
-    scorer: Optional[Callable],
-    threshold: float,
-    max_positive: Optional[int],
-    save_activations: bool,
-) -> "SpanCategorizer":
-    """Create a SpanCategorizer component. The span categorizer consists of two
-    parts: a suggester function that proposes candidate spans, and a labeller
-    model that predicts one or more labels for each span.
-
-    suggester (Callable[[Iterable[Doc], Optional[Ops]], Ragged]): A function that suggests spans.
-        Spans are returned as a ragged array with two integer columns, for the
-        start and end positions.
-    model (Model[Tuple[List[Doc], Ragged], Floats2d]): A model instance that
-        is given a list of documents and (start, end) indices representing
-        candidate span offsets. The model predicts a probability for each category
-        for each span.
-    spans_key (str): Key of the doc.spans dict to save the spans under. During
-        initialization and training, the component will look for spans on the
-        reference document under the same key.
-    scorer (Optional[Callable]): The scoring method. Defaults to
-        Scorer.score_spans for the Doc.spans[spans_key] with overlapping
-        spans allowed.
-    threshold (float): Minimum probability to consider a prediction positive.
-        Spans with a positive prediction will be saved on the Doc. Defaults to
-        0.5.
-    max_positive (Optional[int]): Maximum number of labels to consider positive
-        per span. Defaults to None, indicating no limit.
-        save_activations (bool): save model activations in Doc when annotating.
-    """
-    return SpanCategorizer(
-        nlp.vocab,
-        suggester=suggester,
-        model=model,
-        spans_key=spans_key,
-        threshold=threshold,
-        max_positive=max_positive,
-        name=name,
-        scorer=scorer,
-        save_activations=save_activations,
-    )
-
-
-def spancat_score(examples: Iterable[Example], **kwargs) -> Dict[str, Any]:
-    kwargs = dict(kwargs)
-    attr_prefix = "spans_"
-    key = kwargs["spans_key"]
-    kwargs.setdefault("attr", f"{attr_prefix}{key}")
-    kwargs.setdefault("allow_overlap", True)
-    kwargs.setdefault(
-        "getter", lambda doc, key: doc.spans.get(key[len(attr_prefix) :], [])
-    )
-    kwargs.setdefault("has_annotation", lambda doc: key in doc.spans)
-    return Scorer.score_spans(examples, **kwargs)
-
-
-@registry.scorers("spacy.spancat_scorer.v1")
-def make_spancat_scorer():
-    return spancat_score
+from ..language import Language
+from ..training import Example
 
 
-class SpanCategorizer(TrainablePipe):
-    """Pipeline component to label spans of text.
+cdef class TrainablePipe(Pipe):
+    """This class is a base class and not instantiated directly. Trainable
+    pipeline components like the EntityRecognizer or TextCategorizer inherit
+    from it and it defines the interface that components should follow to
+    function as trainable components in a spaCy pipeline.
 
-    DOCS: https://spacy.io/api/spancategorizer
+    DOCS: https://spacy.io/api/pipe
     """
+    def __init__(self, vocab: Vocab, model: Model, name: str, **cfg):
+        """Initialize a pipeline component.
 
-    def __init__(
-        self,
-        vocab: Vocab,
-        model: Model[Tuple[List[Doc], Ragged], Floats2d],
-        suggester: Suggester,
-        name: str = "spancat",
-        *,
-        spans_key: str = "spans",
-        threshold: float = 0.5,
-        max_positive: Optional[int] = None,
-        scorer: Optional[Callable] = spancat_score,
-        save_activations: bool = False,
-    ) -> None:
-        """Initialize the span categorizer.
         vocab (Vocab): The shared vocabulary.
         model (thinc.api.Model): The Thinc Model powering the pipeline component.
-        name (str): The component instance name, used to add entries to the
-            losses during training.
-        spans_key (str): Key of the Doc.spans dict to save the spans under.
-            During initialization and training, the component will look for
-            spans on the reference document under the same key. Defaults to
-            `"spans"`.
-        threshold (float): Minimum probability to consider a prediction
-            positive. Spans with a positive prediction will be saved on the Doc.
-            Defaults to 0.5.
-        max_positive (Optional[int]): Maximum number of labels to consider
-            positive per span. Defaults to None, indicating no limit.
-        scorer (Optional[Callable]): The scoring method. Defaults to
-            Scorer.score_spans for the Doc.spans[spans_key] with overlapping
-            spans allowed.
-
-        DOCS: https://spacy.io/api/spancategorizer#init
-        """
-        self.cfg = {
-            "labels": [],
-            "spans_key": spans_key,
-            "threshold": threshold,
-            "max_positive": max_positive,
-        }
+        name (str): The component instance name.
+        **cfg: Additional settings and config parameters.
+
+        DOCS: https://spacy.io/api/pipe#init
+        """
         self.vocab = vocab
-        self.suggester = suggester
         self.model = model
         self.name = name
-        self.scorer = scorer
-        self.save_activations = save_activations
-
-    @property
-    def key(self) -> str:
-        """Key of the doc.spans dict to save the spans under. During
-        initialization and training, the component will look for spans on the
-        reference document under the same key.
-        """
-        return str(self.cfg["spans_key"])
-
-    def add_label(self, label: str) -> int:
-        """Add a new label to the pipe.
-
-        label (str): The label to add.
-        RETURNS (int): 0 if label is already present, otherwise 1.
-
-        DOCS: https://spacy.io/api/spancategorizer#add_label
-        """
-        if not isinstance(label, str):
-            raise ValueError(Errors.E187)
-        if label in self.labels:
-            return 0
-        self._allow_extra_label()
-        self.cfg["labels"].append(label)  # type: ignore
-        self.vocab.strings.add(label)
-        return 1
-
-    @property
-    def labels(self) -> Tuple[str]:
-        """RETURNS (Tuple[str]): The labels currently added to the component.
+        self.cfg = dict(cfg)
 
-        DOCS: https://spacy.io/api/spancategorizer#labels
-        """
-        return tuple(self.cfg["labels"])  # type: ignore
-
-    @property
-    def label_data(self) -> List[str]:
-        """RETURNS (List[str]): Information about the component's labels.
+    def __call__(self, Doc doc) -> Doc:
+        """Apply the pipe to one document. The document is modified in place,
+        and returned. This usually happens under the hood when the nlp object
+        is called on a text and all components are applied to the Doc.
+
+        docs (Doc): The Doc to process.
+        RETURNS (Doc): The processed Doc.
+
+        DOCS: https://spacy.io/api/pipe#call
+        """
+        error_handler = self.get_error_handler()
+        try:
+            scores = self.predict([doc])
+            self.set_annotations([doc], scores)
+            return doc
+        except Exception as e:
+            error_handler(self.name, self, [doc], e)
+
+
+    def distill(self,
+               teacher_pipe: Optional["TrainablePipe"],
+               examples: Iterable["Example"],
+               *,
+               drop: float=0.0,
+               sgd: Optional[Optimizer]=None,
+               losses: Optional[Dict[str, float]]=None) -> Dict[str, float]:
+        """Train a pipe (the student) on the predictions of another pipe
+        (the teacher). The student is typically trained on the probability
+        distribution of the teacher, but details may differ per pipe.
+
+        teacher_pipe (Optional[TrainablePipe]): The teacher pipe to learn
+            from.
+        examples (Iterable[Example]): Distillation examples. The reference
+            (teacher) and predicted (student) docs must have the same number of
+            tokens and the same orthography.
+        drop (float): dropout rate.
+        sgd (Optional[Optimizer]): An optimizer. Will be created via
+            create_optimizer if not set.
+        losses (Optional[Dict[str, float]]): Optional record of loss during
+            distillation.
+        RETURNS: The updated losses dictionary.
+        
+        DOCS: https://spacy.io/api/pipe#distill
+        """
+        # By default we require a teacher pipe, but there are downstream
+        # implementations that don't require a pipe.
+        if teacher_pipe is None:
+            raise ValueError(Errors.E4002.format(name=self.name))
+        if losses is None:
+            losses = {}
+        losses.setdefault(self.name, 0.0)
+        validate_distillation_examples(examples, "TrainablePipe.distill")
+        set_dropout_rate(self.model, drop)
+        for node in teacher_pipe.model.walk():
+            if node.name == "softmax":
+                node.attrs["softmax_normalize"] = True
+        teacher_scores = teacher_pipe.model.predict([eg.reference for eg in examples])
+        student_scores, bp_student_scores = self.model.begin_update([eg.predicted for eg in examples])
+        loss, d_scores = self.get_teacher_student_loss(teacher_scores, student_scores)
+        bp_student_scores(d_scores)
+        if sgd is not None:
+            self.finish_update(sgd)
+        losses[self.name] += loss
+        return losses
 
-        DOCS: https://spacy.io/api/spancategorizer#label_data
-        """
-        return list(self.labels)
+    def pipe(self, stream: Iterable[Doc], *, batch_size: int=128) -> Iterator[Doc]:
+        """Apply the pipe to a stream of documents. This usually happens under
+        the hood when the nlp object is called on a text and all components are
+        applied to the Doc.
+
+        stream (Iterable[Doc]): A stream of documents.
+        batch_size (int): The number of documents to buffer.
+        error_handler (Callable[[str, List[Doc], Exception], Any]): Function that
+            deals with a failing batch of documents. The default function just reraises
+            the exception.
+        YIELDS (Doc): Processed documents in order.
+
+        DOCS: https://spacy.io/api/pipe#pipe
+        """
+        error_handler = self.get_error_handler()
+        for docs in util.minibatch(stream, size=batch_size):
+            try:
+                scores = self.predict(docs)
+                self.set_annotations(docs, scores)
+                yield from docs
+            except Exception as e:
+                error_handler(self.name, self, docs, e)
 
-    def predict(self, docs: Iterable[Doc]) -> ActivationsT:
+    def predict(self, docs: Iterable[Doc]):
         """Apply the pipeline's model to a batch of docs, without modifying them.
+        Returns a single tensor for a batch of documents.
 
         docs (Iterable[Doc]): The documents to predict.
-        RETURNS: The models prediction for each document.
+        RETURNS: Vector representations of the predictions.
 
-        DOCS: https://spacy.io/api/spancategorizer#predict
+        DOCS: https://spacy.io/api/pipe#predict
         """
-        indices = self.suggester(docs, ops=self.model.ops)
-        if indices.lengths.sum() == 0:
-            scores = self.model.ops.alloc2f(0, 0)
-        else:
-            scores = self.model.predict((docs, indices))  # type: ignore
-        return {"indices": indices, "scores": scores}
+        raise NotImplementedError(Errors.E931.format(parent="TrainablePipe", method="predict", name=self.name))
 
-    def set_candidates(
-        self, docs: Iterable[Doc], *, candidates_key: str = "candidates"
-    ) -> None:
-        """Use the spancat suggester to add a list of span candidates to a list of docs.
-        This method is intended to be used for debugging purposes.
+    def set_annotations(self, docs: Iterable[Doc], scores):
+        """Modify a batch of documents, using pre-computed scores.
 
         docs (Iterable[Doc]): The documents to modify.
-        candidates_key (str): Key of the Doc.spans dict to save the candidate spans under.
+        scores: The scores to assign.
 
-        DOCS: https://spacy.io/api/spancategorizer#set_candidates
+        DOCS: https://spacy.io/api/pipe#set_annotations
         """
-        suggester_output = self.suggester(docs, ops=self.model.ops)
-
-        for candidates, doc in zip(suggester_output, docs):  # type: ignore
-            doc.spans[candidates_key] = []
-            for index in candidates.dataXd:
-                doc.spans[candidates_key].append(doc[index[0] : index[1]])
-
-    def set_annotations(self, docs: Iterable[Doc], activations: ActivationsT) -> None:
-        """Modify a batch of Doc objects, using pre-computed scores.
+        raise NotImplementedError(Errors.E931.format(parent="TrainablePipe", method="set_annotations", name=self.name))
 
-        docs (Iterable[Doc]): The documents to modify.
-        activations: ActivationsT: The activations, produced by SpanCategorizer.predict.
-
-        DOCS: https://spacy.io/api/spancategorizer#set_annotations
-        """
-        labels = self.labels
-
-        indices = activations["indices"]
-        assert isinstance(indices, Ragged)
-        scores = cast(Floats2d, activations["scores"])
-
-        offset = 0
-        for i, doc in enumerate(docs):
-            indices_i = indices[i].dataXd
-            if self.save_activations:
-                doc.activations[self.name] = {}
-                doc.activations[self.name]["indices"] = indices_i
-                doc.activations[self.name]["scores"] = scores[
-                    offset : offset + indices.lengths[i]
-                ]
-            doc.spans[self.key] = self._make_span_group(
-                doc, indices_i, scores[offset : offset + indices.lengths[i]], labels  # type: ignore[arg-type]
-            )
-            offset += indices.lengths[i]
-
-    def update(
-        self,
-        examples: Iterable[Example],
-        *,
-        drop: float = 0.0,
-        sgd: Optional[Optimizer] = None,
-        losses: Optional[Dict[str, float]] = None,
-    ) -> Dict[str, float]:
+    def update(self,
+               examples: Iterable["Example"],
+               *,
+               drop: float=0.0,
+               sgd: Optimizer=None,
+               losses: Optional[Dict[str, float]]=None) -> Dict[str, float]:
         """Learn from a batch of documents and gold-standard information,
         updating the pipe's model. Delegates to predict and get_loss.
 
         examples (Iterable[Example]): A batch of Example objects.
         drop (float): The dropout rate.
         sgd (thinc.api.Optimizer): The optimizer.
         losses (Dict[str, float]): Optional record of the loss during training.
             Updated using the component name as the key.
         RETURNS (Dict[str, float]): The updated losses dictionary.
 
-        DOCS: https://spacy.io/api/spancategorizer#update
+        DOCS: https://spacy.io/api/pipe#update
         """
         if losses is None:
             losses = {}
+        if not hasattr(self, "model") or self.model in (None, True, False):
+            return losses
         losses.setdefault(self.name, 0.0)
-        validate_examples(examples, "SpanCategorizer.update")
-        self._validate_categories(examples)
+        validate_examples(examples, "TrainablePipe.update")
         if not any(len(eg.predicted) if eg.predicted else 0 for eg in examples):
             # Handle cases where there are no tokens in any docs.
             return losses
-        docs = [eg.predicted for eg in examples]
-        spans = self.suggester(docs, ops=self.model.ops)
-        if spans.lengths.sum() == 0:
-            return losses
         set_dropout_rate(self.model, drop)
-        scores, backprop_scores = self.model.begin_update((docs, spans))
-        loss, d_scores = self.get_loss(examples, (spans, scores))
-        backprop_scores(d_scores)  # type: ignore
-        if sgd is not None:
+        scores, bp_scores = self.model.begin_update([eg.predicted for eg in examples])
+        loss, d_scores = self.get_loss(examples, scores)
+        bp_scores(d_scores)
+        if sgd not in (None, False):
             self.finish_update(sgd)
         losses[self.name] += loss
         return losses
 
-    def get_loss(
-        self, examples: Iterable[Example], spans_scores: Tuple[Ragged, Floats2d]
-    ) -> Tuple[float, float]:
+    def rehearse(self,
+                 examples: Iterable[Example],
+                 *,
+                 sgd: Optimizer=None,
+                 losses: Dict[str, float]=None,
+                 **config) -> Dict[str, float]:
+        """Perform a "rehearsal" update from a batch of data. Rehearsal updates
+        teach the current model to make predictions similar to an initial model,
+        to try to address the "catastrophic forgetting" problem. This feature is
+        experimental.
+
+        examples (Iterable[Example]): A batch of Example objects.
+        sgd (thinc.api.Optimizer): The optimizer.
+        losses (Dict[str, float]): Optional record of the loss during training.
+            Updated using the component name as the key.
+        RETURNS (Dict[str, float]): The updated losses dictionary.
+
+        DOCS: https://spacy.io/api/pipe#rehearse
+        """
+        pass
+
+    def get_loss(self, examples: Iterable[Example], scores) -> Tuple[float, float]:
         """Find the loss and gradient of loss for the batch of documents and
         their predicted scores.
 
         examples (Iterable[Examples]): The batch of examples.
-        spans_scores: Scores representing the model's predictions.
+        scores: Scores representing the model's predictions.
         RETURNS (Tuple[float, float]): The loss and the gradient.
 
-        DOCS: https://spacy.io/api/spancategorizer#get_loss
+        DOCS: https://spacy.io/api/pipe#get_loss
         """
-        spans, scores = spans_scores
-        spans = Ragged(
-            self.model.ops.to_numpy(spans.data), self.model.ops.to_numpy(spans.lengths)
-        )
-        label_map = {label: i for i, label in enumerate(self.labels)}
-        target = numpy.zeros(scores.shape, dtype=scores.dtype)
-        offset = 0
-        for i, eg in enumerate(examples):
-            # Map (start, end) offset of spans to the row in the d_scores array,
-            # so that we can adjust the gradient for predictions that were
-            # in the gold standard.
-            spans_index = {}
-            spans_i = spans[i].dataXd
-            for j in range(spans.lengths[i]):
-                start = int(spans_i[j, 0])  # type: ignore
-                end = int(spans_i[j, 1])  # type: ignore
-                spans_index[(start, end)] = offset + j
-            for gold_span in self._get_aligned_spans(eg):
-                key = (gold_span.start, gold_span.end)
-                if key in spans_index:
-                    row = spans_index[key]
-                    k = label_map[gold_span.label_]
-                    target[row, k] = 1.0
-            # The target is a flat array for all docs. Track the position
-            # we're at within the flat array.
-            offset += spans.lengths[i]
-        target = self.model.ops.asarray(target, dtype="f")  # type: ignore
-        # The target will have the values 0 (for untrue predictions) or 1
-        # (for true predictions).
-        # The scores should be in the range [0, 1].
-        # If the prediction is 0.9 and it's true, the gradient
-        # will be -0.1 (0.9 - 1.0).
-        # If the prediction is 0.9 and it's false, the gradient will be
-        # 0.9 (0.9 - 0.0)
-        d_scores = scores - target
-        loss = float((d_scores**2).sum())
-        return loss, d_scores
-
-    def initialize(
-        self,
-        get_examples: Callable[[], Iterable[Example]],
-        *,
-        nlp: Optional[Language] = None,
-        labels: Optional[List[str]] = None,
-    ) -> None:
-        """Initialize the pipe for training, using a representative set
-        of data examples.
+        raise NotImplementedError(Errors.E931.format(parent="TrainablePipe", method="get_loss", name=self.name))
+
+    def get_teacher_student_loss(self, teacher_scores, student_scores):
+        """Calculate the loss and its gradient for a batch of student
+        scores, relative to teacher scores.
+
+        teacher_scores: Scores representing the teacher model's predictions.
+        student_scores: Scores representing the student model's predictions.
+
+        RETURNS (Tuple[float, float]): The loss and the gradient.
+        
+        DOCS: https://spacy.io/api/pipe#get_teacher_student_loss
+        """
+        raise NotImplementedError(Errors.E931.format(parent="TrainablePipe", method="get_teacher_student_loss", name=self.name))
+
+    def create_optimizer(self) -> Optimizer:
+        """Create an optimizer for the pipeline component.
+
+        RETURNS (thinc.api.Optimizer): The optimizer.
+
+        DOCS: https://spacy.io/api/pipe#create_optimizer
+        """
+        return util.create_default_optimizer()
+
+    def initialize(self, get_examples: Callable[[], Iterable[Example]], *, nlp: Language=None):
+        """Initialize the pipe for training, using data examples if available.
+        This method needs to be implemented by each TrainablePipe component,
+        ensuring the internal model (if available) is initialized properly
+        using the provided sample of Example objects.
 
         get_examples (Callable[[], Iterable[Example]]): Function that
             returns a representative sample of gold-standard Example objects.
-        nlp (Optional[Language]): The current nlp object the component is part of.
-        labels (Optional[List[str]]): The labels to add to the component, typically generated by the
-            `init labels` command. If no labels are provided, the get_examples
-            callback is used to extract the labels from the data.
-
-        DOCS: https://spacy.io/api/spancategorizer#initialize
-        """
-        subbatch: List[Example] = []
-        if labels is not None:
-            for label in labels:
-                self.add_label(label)
-        for eg in get_examples():
-            if labels is None:
-                for span in eg.reference.spans.get(self.key, []):
-                    self.add_label(span.label_)
-            if len(subbatch) < 10:
-                subbatch.append(eg)
-        self._require_labels()
-        if subbatch:
-            docs = [eg.x for eg in subbatch]
-            spans = build_ngram_suggester(sizes=[1])(docs)
-            Y = self.model.ops.alloc2f(spans.dataXd.shape[0], len(self.labels))
-            self.model.initialize(X=(docs, spans), Y=Y)
+        nlp (Language): The current nlp object the component is part of.
+
+        DOCS: https://spacy.io/api/pipe#initialize
+        """
+        raise NotImplementedError(Errors.E931.format(parent="TrainablePipe", method="initialize", name=self.name))
+
+    def add_label(self, label: str) -> int:
+        """Add an output label.
+        For TrainablePipe components, it is possible to
+        extend pretrained models with new labels, but care should be taken to
+        avoid the "catastrophic forgetting" problem.
+
+        label (str): The label to add.
+        RETURNS (int): 0 if label is already present, otherwise 1.
+
+        DOCS: https://spacy.io/api/pipe#add_label
+        """
+        raise NotImplementedError(Errors.E931.format(parent="Pipe", method="add_label", name=self.name))
+
+    @property
+    def is_distillable(self) -> bool:
+        # Normally a pipe overrides `get_teacher_student_loss` to implement
+        # distillation. In more exceptional cases, a pipe can provide its
+        # own `distill` implementation. If neither of these methods is
+        # overridden, the pipe does not implement distillation.
+        return not (self.__class__.distill is TrainablePipe.distill and self.__class__.get_teacher_student_loss is TrainablePipe.get_teacher_student_loss)
+
+    @property
+    def is_trainable(self) -> bool:
+        return True
+
+    @property
+    def is_resizable(self) -> bool:
+        return getattr(self, "model", None) and "resize_output" in self.model.attrs
+
+    def _allow_extra_label(self) -> None:
+        """Raise an error if the component can not add any more labels."""
+        nO = None
+        if self.model.has_dim("nO"):
+            nO = self.model.get_dim("nO")
+        elif self.model.has_ref("output_layer") and self.model.get_ref("output_layer").has_dim("nO"):
+            nO = self.model.get_ref("output_layer").get_dim("nO")
+        if nO is not None and nO == len(self.labels):
+            if not self.is_resizable:
+                raise ValueError(Errors.E922.format(name=self.name, nO=self.model.get_dim("nO")))
+
+    def set_output(self, nO: int) -> None:
+        if self.is_resizable:
+            self.model.attrs["resize_output"](self.model, nO)
         else:
-            self.model.initialize()
+            raise NotImplementedError(Errors.E921)
 
-    def _validate_categories(self, examples: Iterable[Example]):
-        # TODO
-        pass
+    def use_params(self, params: dict):
+        """Modify the pipe's model, to use the given parameter values. At the
+        end of the context, the original parameters are restored.
+
+        params (dict): The parameter values to use in the model.
+
+        DOCS: https://spacy.io/api/pipe#use_params
+        """
+        with self.model.use_params(params):
+            yield
+
+    def finish_update(self, sgd: Optimizer) -> None:
+        """Update parameters using the current parameter gradients.
+        The Optimizer instance contains the functionality to perform
+        the stochastic gradient descent.
 
-    def _get_aligned_spans(self, eg: Example):
-        return eg.get_aligned_spans_y2x(
-            eg.reference.spans.get(self.key, []), allow_overlap=True
-        )
-
-    def _make_span_group(
-        self, doc: Doc, indices: Ints2d, scores: Floats2d, labels: List[str]
-    ) -> SpanGroup:
-        spans = SpanGroup(doc, name=self.key)
-        max_positive = self.cfg["max_positive"]
-        threshold = self.cfg["threshold"]
-
-        keeps = scores >= threshold
-        ranked = (scores * -1).argsort()  # type: ignore
-        if max_positive is not None:
-            assert isinstance(max_positive, int)
-            span_filter = ranked[:, max_positive:]
-            for i, row in enumerate(span_filter):
-                keeps[i, row] = False
-        spans.attrs["scores"] = scores[keeps].flatten()
-
-        indices = self.model.ops.to_numpy(indices)
-        keeps = self.model.ops.to_numpy(keeps)
-
-        for i in range(indices.shape[0]):
-            start = indices[i, 0]
-            end = indices[i, 1]
-
-            for j, keep in enumerate(keeps[i]):
-                if keep:
-                    spans.append(Span(doc, start, end, label=labels[j]))
+        sgd (thinc.api.Optimizer): The optimizer.
+
+        DOCS: https://spacy.io/api/pipe#finish_update
+        """
+        self.model.finish_update(sgd)
+
+    def _validate_serialization_attrs(self):
+        """Check that the pipe implements the required attributes. If a subclass
+        implements a custom __init__ method but doesn't set these attributes,
+        they currently default to None, so we need to perform additonal checks.
+        """
+        if not hasattr(self, "vocab") or self.vocab is None:
+            raise ValueError(Errors.E899.format(name=util.get_object_name(self)))
+        if not hasattr(self, "model") or self.model is None:
+            raise ValueError(Errors.E898.format(name=util.get_object_name(self)))
+
+    def to_bytes(self, *, exclude=tuple()):
+        """Serialize the pipe to a bytestring.
+
+        exclude (Iterable[str]): String names of serialization fields to exclude.
+        RETURNS (bytes): The serialized object.
+
+        DOCS: https://spacy.io/api/pipe#to_bytes
+        """
+        self._validate_serialization_attrs()
+        serialize = {}
+        if hasattr(self, "cfg") and self.cfg is not None:
+            serialize["cfg"] = lambda: srsly.json_dumps(self.cfg)
+        serialize["vocab"] = lambda: self.vocab.to_bytes(exclude=exclude)
+        serialize["model"] = self.model.to_bytes
+        return util.to_bytes(serialize, exclude)
+
+    def from_bytes(self, bytes_data, *, exclude=tuple()):
+        """Load the pipe from a bytestring.
+
+        exclude (Iterable[str]): String names of serialization fields to exclude.
+        RETURNS (TrainablePipe): The loaded object.
+
+        DOCS: https://spacy.io/api/pipe#from_bytes
+        """
+        self._validate_serialization_attrs()
+
+        def load_model(b):
+            try:
+                self.model.from_bytes(b)
+            except AttributeError:
+                raise ValueError(Errors.E149) from None
+
+        deserialize = {}
+        if hasattr(self, "cfg") and self.cfg is not None:
+            deserialize["cfg"] = lambda b: self.cfg.update(srsly.json_loads(b))
+        deserialize["vocab"] = lambda b: self.vocab.from_bytes(b, exclude=exclude)
+        deserialize["model"] = load_model
+        util.from_bytes(bytes_data, deserialize, exclude)
+        return self
+
+    def to_disk(self, path, *, exclude=tuple()):
+        """Serialize the pipe to disk.
+
+        path (str / Path): Path to a directory.
+        exclude (Iterable[str]): String names of serialization fields to exclude.
+
+        DOCS: https://spacy.io/api/pipe#to_disk
+        """
+        self._validate_serialization_attrs()
+        serialize = {}
+        if hasattr(self, "cfg") and self.cfg is not None:
+            serialize["cfg"] = lambda p: srsly.write_json(p, self.cfg)
+        serialize["vocab"] = lambda p: self.vocab.to_disk(p, exclude=exclude)
+        serialize["model"] = lambda p: self.model.to_disk(p)
+        util.to_disk(path, serialize, exclude)
+
+    def from_disk(self, path, *, exclude=tuple()):
+        """Load the pipe from disk.
+
+        path (str / Path): Path to a directory.
+        exclude (Iterable[str]): String names of serialization fields to exclude.
+        RETURNS (TrainablePipe): The loaded object.
+
+        DOCS: https://spacy.io/api/pipe#from_disk
+        """
+        self._validate_serialization_attrs()
+
+        def load_model(p):
+            try:
+                with open(p, "rb") as mfile:
+                    self.model.from_bytes(mfile.read())
+            except AttributeError:
+                raise ValueError(Errors.E149) from None
+
+        deserialize = {}
+        if hasattr(self, "cfg") and self.cfg is not None:
+            deserialize["cfg"] = lambda p: self.cfg.update(deserialize_config(p))
+        deserialize["vocab"] = lambda p: self.vocab.from_disk(p, exclude=exclude)
+        deserialize["model"] = load_model
+        util.from_disk(path, deserialize, exclude)
+        return self
+
+    @property
+    def save_activations(self):
+        return self._save_activations
 
-        return spans
+    @save_activations.setter
+    def save_activations(self, save_activations: bool):
+        self._save_activations = save_activations
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/tagger.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/tagger.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,14 @@
 from ..training import validate_examples, validate_get_examples
 from ..util import registry
 from .. import util
 
 
 ActivationsT = Dict[str, Union[List[Floats2d], List[Ints1d]]]
 
-# See #9050
-BACKWARD_OVERWRITE = False
-
 default_model_config = """
 [model]
 @architectures = "spacy.Tagger.v2"
 
 [model.tok2vec]
 @architectures = "spacy.HashEmbedCNN.v2"
 pretrained_vectors = null
@@ -51,36 +48,38 @@
     "tagger",
     assigns=["token.tag"],
     default_config={
         "model": DEFAULT_TAGGER_MODEL,
         "overwrite": False,
         "scorer": {"@scorers": "spacy.tagger_scorer.v1"},
         "neg_prefix": "!",
+        "label_smoothing": 0.0,
         "save_activations": False,
     },
     default_score_weights={"tag_acc": 1.0},
 )
 def make_tagger(
     nlp: Language,
     name: str,
     model: Model,
     overwrite: bool,
     scorer: Optional[Callable],
     neg_prefix: str,
+    label_smoothing: float,
     save_activations: bool,
 ):
     """Construct a part-of-speech tagger component.
 
     model (Model[List[Doc], List[Floats2d]]): A model instance that predicts
         the tag probabilities. The output vectors should match the number of tags
         in size, and be normalized as probabilities (all scores between 0 and 1,
         with the rows summing to 1).
     """
     return Tagger(nlp.vocab, model, name, overwrite=overwrite, scorer=scorer, neg_prefix=neg_prefix,
-                  save_activations=save_activations)
+                  label_smoothing=label_smoothing, save_activations=save_activations)
 
 
 def tagger_score(examples, **kwargs):
     return Scorer.score_token_attr(examples, "tag", **kwargs)
 
 
 @registry.scorers("spacy.tagger_scorer.v1")
@@ -95,36 +94,43 @@
     """
     def __init__(
         self,
         vocab,
         model,
         name="tagger",
         *,
-        overwrite=BACKWARD_OVERWRITE,
+        overwrite=False,
         scorer=tagger_score,
         neg_prefix="!",
+        label_smoothing=0.0,
         save_activations: bool = False,
     ):
         """Initialize a part-of-speech tagger.
 
         vocab (Vocab): The shared vocabulary.
         model (thinc.api.Model): The Thinc Model powering the pipeline component.
         name (str): The component instance name, used to add entries to the
             losses during training.
+        overwrite (bool): Whether to overwrite existing annotations.
         scorer (Optional[Callable]): The scoring method. Defaults to
             Scorer.score_token_attr for the attribute "tag".
         save_activations (bool): save model activations in Doc when annotating.
 
         DOCS: https://spacy.io/api/tagger#init
         """
         self.vocab = vocab
         self.model = model
         self.name = name
         self._rehearsal_model = None
-        cfg = {"labels": [], "overwrite": overwrite, "neg_prefix": neg_prefix}
+        cfg = {
+            "labels": [],
+            "overwrite": overwrite,
+            "neg_prefix": neg_prefix,
+            "label_smoothing": label_smoothing
+        }
         self.cfg = dict(sorted(cfg.items()))
         self.scorer = scorer
         self.save_activations = save_activations
 
     @property
     def labels(self):
         """The labels currently added to the component. Note that even for a
@@ -292,15 +298,20 @@
         examples (Iterable[Examples]): The batch of examples.
         scores: Scores representing the model's predictions.
         RETURNS (Tuple[float, float]): The loss and the gradient.
 
         DOCS: https://spacy.io/api/tagger#get_loss
         """
         validate_examples(examples, "Tagger.get_loss")
-        loss_func = LegacySequenceCategoricalCrossentropy(names=self.labels, normalize=False, neg_prefix=self.cfg["neg_prefix"])
+        loss_func = LegacySequenceCategoricalCrossentropy(
+            names=self.labels,
+            normalize=False,
+            neg_prefix=self.cfg["neg_prefix"],
+            label_smoothing=self.cfg["label_smoothing"]
+        )
         # Convert empty tag "" to missing value None so that both misaligned
         # tokens and tokens with missing annotation have the default missing
         # value None.
         truths = []
         for eg in examples:
             eg_truths = [tag if tag is not "" else None for tag in eg.get_aligned("TAG", as_string=True)]
             truths.append(eg_truths)
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/textcat.py` & `spacy-4.0.0.dev1/spacy/pipeline/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/textcat_multilabel.py` & `spacy-4.0.0.dev1/spacy/pipeline/textcat_multilabel.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/tok2vec.py` & `spacy-4.0.0.dev1/spacy/pipeline/tok2vec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Sequence, Iterable, Optional, Dict, Callable, List, Any
+from typing import Sequence, Iterable, Optional, Dict, Callable, List, Any, Tuple
 from thinc.api import Model, set_dropout_rate, Optimizer, Config
+from thinc.types import Floats2d
 from itertools import islice
 
 from .trainable_pipe import TrainablePipe
 from ..training import Example, validate_examples, validate_get_examples
 from ..tokens import Doc
 from ..vocab import Vocab
 from ..language import Language
@@ -153,47 +154,17 @@
         sgd (thinc.api.Optimizer): The optimizer.
         losses (Dict[str, float]): Optional record of the loss during training.
             Updated using the component name as the key.
         RETURNS (Dict[str, float]): The updated losses dictionary.
 
         DOCS: https://spacy.io/api/tok2vec#update
         """
-        if losses is None:
-            losses = {}
         validate_examples(examples, "Tok2Vec.update")
         docs = [eg.predicted for eg in examples]
-        set_dropout_rate(self.model, drop)
-        tokvecs, bp_tokvecs = self.model.begin_update(docs)
-        d_tokvecs = [self.model.ops.alloc2f(*t2v.shape) for t2v in tokvecs]
-        losses.setdefault(self.name, 0.0)
-
-        def accumulate_gradient(one_d_tokvecs):
-            """Accumulate tok2vec loss and gradient. This is passed as a callback
-            to all but the last listener. Only the last one does the backprop.
-            """
-            nonlocal d_tokvecs
-            for i in range(len(one_d_tokvecs)):
-                d_tokvecs[i] += one_d_tokvecs[i]
-                losses[self.name] += float((one_d_tokvecs[i] ** 2).sum())
-            return [self.model.ops.alloc2f(*t2v.shape) for t2v in tokvecs]
-
-        def backprop(one_d_tokvecs):
-            """Callback to actually do the backprop. Passed to last listener."""
-            accumulate_gradient(one_d_tokvecs)
-            d_docs = bp_tokvecs(d_tokvecs)
-            if sgd is not None:
-                self.finish_update(sgd)
-            return d_docs
-
-        batch_id = Tok2VecListener.get_batch_id(docs)
-        for listener in self.listeners[:-1]:
-            listener.receive(batch_id, tokvecs, accumulate_gradient)
-        if self.listeners:
-            self.listeners[-1].receive(batch_id, tokvecs, backprop)
-        return losses
+        return self._update_with_docs(docs, drop=drop, sgd=sgd, losses=losses)
 
     def get_loss(self, examples, scores) -> None:
         pass
 
     def initialize(
         self,
         get_examples: Callable[[], Iterable[Example]],
@@ -215,14 +186,104 @@
             doc_sample.append(example.x)
         assert doc_sample, Errors.E923.format(name=self.name)
         self.model.initialize(X=doc_sample)
 
     def add_label(self, label):
         raise NotImplementedError
 
+    def distill(
+        self,
+        teacher_pipe: Optional["TrainablePipe"],
+        examples: Iterable["Example"],
+        *,
+        drop: float = 0.0,
+        sgd: Optional[Optimizer] = None,
+        losses: Optional[Dict[str, float]] = None,
+    ) -> Dict[str, float]:
+        """Performs an update of the student pipe's model using the
+        student's distillation examples and sets the annotations
+        of the teacher's distillation examples using the teacher pipe.
+
+        teacher_pipe (Optional[TrainablePipe]): The teacher pipe to use
+            for prediction.
+        examples (Iterable[Example]): Distillation examples. The reference (teacher)
+            and predicted (student) docs must have the same number of tokens and the
+            same orthography.
+        drop (float): dropout rate.
+        sgd (Optional[Optimizer]): An optimizer. Will be created via
+            create_optimizer if not set.
+        losses (Optional[Dict[str, float]]): Optional record of loss during
+            distillation.
+        RETURNS: The updated losses dictionary.
+
+        DOCS: https://spacy.io/api/tok2vec#distill
+        """
+        # By default we require a teacher pipe, but there are downstream
+        # implementations that don't require a pipe.
+        if teacher_pipe is None:
+            raise ValueError(Errors.E4002.format(name=self.name))
+        teacher_docs = [eg.reference for eg in examples]
+        student_docs = [eg.predicted for eg in examples]
+        teacher_preds = teacher_pipe.predict(teacher_docs)
+        teacher_pipe.set_annotations(teacher_docs, teacher_preds)
+        return self._update_with_docs(student_docs, drop=drop, sgd=sgd, losses=losses)
+
+    def _update_with_docs(
+        self,
+        docs: Iterable[Doc],
+        *,
+        drop: float = 0.0,
+        sgd: Optional[Optimizer] = None,
+        losses: Optional[Dict[str, float]] = None,
+    ):
+        if losses is None:
+            losses = {}
+        losses.setdefault(self.name, 0.0)
+        set_dropout_rate(self.model, drop)
+
+        tokvecs, accumulate_gradient, backprop = self._create_backprops(
+            docs, losses, sgd=sgd
+        )
+        batch_id = Tok2VecListener.get_batch_id(docs)
+        for listener in self.listeners[:-1]:
+            listener.receive(batch_id, tokvecs, accumulate_gradient)
+        if self.listeners:
+            self.listeners[-1].receive(batch_id, tokvecs, backprop)
+        return losses
+
+    def _create_backprops(
+        self,
+        docs: Iterable[Doc],
+        losses: Dict[str, float],
+        *,
+        sgd: Optional[Optimizer] = None,
+    ) -> Tuple[Floats2d, Callable, Callable]:
+        tokvecs, bp_tokvecs = self.model.begin_update(docs)
+        d_tokvecs = [self.model.ops.alloc2f(*t2v.shape) for t2v in tokvecs]
+
+        def accumulate_gradient(one_d_tokvecs):
+            """Accumulate tok2vec loss and gradient. This is passed as a callback
+            to all but the last listener. Only the last one does the backprop.
+            """
+            nonlocal d_tokvecs
+            for i in range(len(one_d_tokvecs)):
+                d_tokvecs[i] += one_d_tokvecs[i]
+                losses[self.name] += float((one_d_tokvecs[i] ** 2).sum())
+            return [self.model.ops.alloc2f(*t2v.shape) for t2v in tokvecs]
+
+        def backprop(one_d_tokvecs):
+            """Callback to actually do the backprop. Passed to last listener."""
+            accumulate_gradient(one_d_tokvecs)
+            d_docs = bp_tokvecs(d_tokvecs)
+            if sgd is not None:
+                self.finish_update(sgd)
+            return d_docs
+
+        return tokvecs, accumulate_gradient, backprop
+
 
 class Tok2VecListener(Model):
     """A layer that gets fed its answers from an upstream connection,
     for instance from a component earlier in the pipeline.
 
     The Tok2VecListener layer is used as a sublayer within a component such
     as a parser, NER or text categorizer. Usually you'll have multiple listeners
```

### Comparing `spacy-4.0.0.dev0/spacy/pipeline/transition_parser.pyx` & `spacy-4.0.0.dev1/spacy/pipeline/transition_parser.pyx`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,19 @@
 
 from ..training import validate_examples, validate_get_examples
 from ..training import validate_distillation_examples
 from ..errors import Errors, Warnings
 from .. import util
 
 
+# TODO: Remove when we switch to Cython 3.
+cdef extern from "<algorithm>" namespace "std" nogil:
+    bint equal[InputIt1, InputIt2](InputIt1 first1, InputIt1 last1, InputIt2 first2) except +
+
+
 NUMPY_OPS = NumpyOps()
 
 
 class Parser(TrainablePipe):
     """
     Base class of the DependencyParser and EntityRecognizer.
     """
@@ -220,16 +225,16 @@
         """Train a pipe (the student) on the predictions of another pipe
         (the teacher). The student is trained on the transition probabilities
         of the teacher.
 
         teacher_pipe (Optional[TrainablePipe]): The teacher pipe to learn
             from.
         examples (Iterable[Example]): Distillation examples. The reference
-            and predicted docs must have the same number of tokens and the
-            same orthography.
+            (teacher) and predicted (student) docs must have the same number of
+            tokens and the same orthography.
         drop (float): dropout rate.
         sgd (Optional[Optimizer]): An optimizer. Will be created via
             create_optimizer if not set.
         losses (Optional[Dict[str, float]]): Optional record of loss during
             distillation.
         RETURNS: The updated losses dictionary.
         
@@ -249,32 +254,32 @@
 
         max_moves = self.cfg["update_with_oracle_cut_size"]
         if max_moves >= 1:
             # Chop sequences into lengths of this many words, to make the
             # batch uniform length. Since we do not have a gold standard
             # sequence, we use the teacher's predictions as the gold
             # standard.
-            max_moves = int(random.uniform(max_moves // 2, max_moves * 2))
-            states = self._init_batch(teacher_pipe, student_docs, max_moves)
+            max_moves = int(random.uniform(max(max_moves // 2, 1), max_moves * 2))
+            states = self._init_batch_from_teacher(teacher_pipe, student_docs, max_moves)
         else:
             states = self.moves.init_batch(student_docs)
 
         # We distill as follows: 1. we first let the student predict transition
         # sequences (and the corresponding transition probabilities); (2) we
         # let the teacher follow the student's predicted transition sequences
         # to obtain the teacher's transition probabilities; (3) we compute the
         # gradients of the student's transition distributions relative to the
         # teacher's distributions.
 
-        student_inputs = TransitionModelInputs(docs=student_docs, moves=self.moves,
-            max_moves=max_moves)
+        student_inputs = TransitionModelInputs(docs=student_docs,
+            states=[state.copy() for state in states], moves=self.moves, max_moves=max_moves)
         (student_states, student_scores), backprop_scores = self.model.begin_update(student_inputs)
-        actions = states2actions(student_states)
+        actions = _states_diff_to_actions(states, student_states)
         teacher_inputs = TransitionModelInputs(docs=[eg.reference for eg in examples],
-            moves=self.moves, actions=actions)
+            states=states, moves=teacher_pipe.moves, actions=actions)
         (_, teacher_scores) = teacher_pipe.model.predict(teacher_inputs)
 
         loss, d_scores = self.get_teacher_student_loss(teacher_scores, student_scores)
         backprop_scores((student_states, d_scores))
 
         if sgd is not None:
             self.finish_update(sgd)
@@ -518,15 +523,15 @@
         # expand our model output.
         self._resize()
         # Prepare the stepwise model, and get the callback for finishing the batch
         set_dropout_rate(self._rehearsal_model, 0.0)
         set_dropout_rate(self.model, 0.0)
         student_inputs = TransitionModelInputs(docs=docs, moves=self.moves)
         (student_states, student_scores), backprop_scores = self.model.begin_update(student_inputs)
-        actions = states2actions(student_states)
+        actions = _states_to_actions(student_states)
         teacher_inputs = TransitionModelInputs(docs=docs, moves=self.moves, actions=actions)
         _, teacher_scores = self._rehearsal_model.predict(teacher_inputs)
 
         loss, d_scores = self.get_teacher_student_loss(teacher_scores, student_scores, normalize=True)
 
         teacher_scores = self.model.ops.xp.vstack(teacher_scores)
         student_scores = self.model.ops.xp.vstack(student_scores)
@@ -638,47 +643,59 @@
             if 'model' in msg:
                 try:
                     self.model.from_bytes(msg['model'])
                 except AttributeError:
                     raise ValueError(Errors.E149) from None
         return self
 
-    def _init_batch(self, teacher_step_model, docs, max_length):
+    def _init_batch_from_teacher(self, teacher_pipe, docs, max_length):
         """Make a square batch of length equal to the shortest transition
         sequence or a cap. A long
         doc will get multiple states. Let's say we have a doc of length 2*N,
         where N is the shortest doc. We'll make two states, one representing
         long_doc[:N], and another representing long_doc[N:]. In contrast to
         _init_gold_batch, this version uses a teacher model to generate the
         cut sequences."""
         cdef:
-            StateClass start_state
             StateClass state
-            Transition action
-        all_states = self.moves.init_batch(docs)
+            TransitionSystem moves = teacher_pipe.moves
+
+        # Start with the same heuristic as in supervised training: exclude
+        # docs that are within the maximum length.
+        all_states = moves.init_batch(docs)
         states = []
         to_cut = []
         for state, doc in zip(all_states, docs):
             if not state.is_final():
                 if len(doc) < max_length:
                     states.append(state)
                 else:
                     to_cut.append(state)
+
+        if not to_cut:
+            return states
+
+        # Parse the states that are too long with the teacher's parsing model.
+        teacher_inputs = TransitionModelInputs(docs=docs, moves=moves,
+            states=[state.copy() for state in to_cut])
+        (teacher_states, _ ) = teacher_pipe.model.predict(teacher_inputs)
+
+        # Step through the teacher's actions and store every state after
+        # each multiple of max_length.
+        teacher_actions = _states_to_actions(teacher_states)
         while to_cut:
             states.extend(state.copy() for state in to_cut)
-            # Move states forward max_length actions.
-            length = 0
-            while to_cut and length < max_length:
-                teacher_scores = teacher_step_model.predict(to_cut)
-                self.transition_states(to_cut, teacher_scores)
-                # States that are completed do not need further cutting.
-                to_cut = [state for state in to_cut if not state.is_final()]
-                length += 1
-        return states
+            for step_actions in teacher_actions[:max_length]:
+                to_cut = moves.apply_actions(to_cut, step_actions)
+            teacher_actions = teacher_actions[max_length:]
 
+            if len(teacher_actions) < max_length:
+                break
+
+        return states
 
     def _init_gold_batch(self, examples, max_length):
         """Make a square batch, of length equal to the shortest transition
         sequence or a cap. A long doc will get multiple states. Let's say we
         have a doc of length 2*N, where N is the shortest doc. We'll make
         two states, one representing long_doc[:N], and another representing
         long_doc[N:]."""
@@ -732,15 +749,15 @@
     for key, value in old_attrs.items():
         if value is unset:
             model.attrs.pop(key)
         else:
             model.attrs[key] = value
 
 
-def states2actions(states: List[StateClass]) -> List[Ints1d]:
+def _states_to_actions(states: List[StateClass]) -> List[Ints1d]:
     cdef int step
     cdef StateClass state
     cdef StateC* c_state
     actions = []
     while True:
         step = len(actions)
 
@@ -752,8 +769,50 @@
 
         # We are done if we have exhausted all histories.
         if len(step_actions) == 0:
             break
 
         actions.append(numpy.array(step_actions, dtype="i"))
 
+    return actions
+
+def _states_diff_to_actions(
+    before_states: List[StateClass],
+    after_states: List[StateClass]
+) -> List[Ints1d]:
+    """
+    Return for two sets of states the actions to go from the first set of
+    states to the second set of states. The histories of the first set of
+    states must be a prefix of the second set of states.
+    """
+    cdef StateClass before_state, after_state
+    cdef StateC* c_state_before
+    cdef StateC* c_state_after
+
+    assert len(before_states) == len(after_states)
+
+    # Check invariant: before states histories must be prefixes of after states.
+    for before_state, after_state in zip(before_states, after_states):
+        c_state_before = before_state.c
+        c_state_after = after_state.c
+
+        assert equal(c_state_before.history.begin(), c_state_before.history.end(),
+            c_state_after.history.begin())
+
+    actions = []
+    while True:
+        step = len(actions)
+
+        step_actions = []
+        for before_state, after_state in zip(before_states, after_states):
+            c_state_before = before_state.c
+            c_state_after = after_state.c
+            if step < c_state_after.history.size() - c_state_before.history.size():
+                step_actions.append(c_state_after.history[c_state_before.history.size() + step])
+
+        # We are done if we have exhausted all histories.
+        if len(step_actions) == 0:
+            break
+
+        actions.append(numpy.array(step_actions, dtype="i"))
+
     return actions
```

### Comparing `spacy-4.0.0.dev0/spacy/schemas.py` & `spacy-4.0.0.dev1/spacy/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Dict, List, Union, Optional, Any, Callable, Type, Tuple
-from typing import Iterable, TypeVar, TYPE_CHECKING
-from .compat import Literal
+from typing import Iterable, TypeVar, Literal, TYPE_CHECKING
 from enum import Enum
 from pydantic import BaseModel, Field, ValidationError, validator, create_model
 from pydantic import StrictStr, StrictInt, StrictFloat, StrictBool, ConstrainedStr
 from pydantic.main import ModelMetaclass
 from thinc.api import Optimizer, ConfigValidationError, Model
 from thinc.config import Promise
 from collections import defaultdict
@@ -159,23 +158,41 @@
     REGEX: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="regex")
     IN: Optional[List[StrictStr]] = Field(None, alias="in")
     NOT_IN: Optional[List[StrictStr]] = Field(None, alias="not_in")
     IS_SUBSET: Optional[List[StrictStr]] = Field(None, alias="is_subset")
     IS_SUPERSET: Optional[List[StrictStr]] = Field(None, alias="is_superset")
     INTERSECTS: Optional[List[StrictStr]] = Field(None, alias="intersects")
     FUZZY: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy")
-    FUZZY1: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy1")
-    FUZZY2: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy2")
-    FUZZY3: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy3")
-    FUZZY4: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy4")
-    FUZZY5: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy5")
-    FUZZY6: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy6")
-    FUZZY7: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy7")
-    FUZZY8: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy8")
-    FUZZY9: Optional[Union[StrictStr, "TokenPatternString"]] = Field(None, alias="fuzzy9")
+    FUZZY1: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy1"
+    )
+    FUZZY2: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy2"
+    )
+    FUZZY3: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy3"
+    )
+    FUZZY4: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy4"
+    )
+    FUZZY5: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy5"
+    )
+    FUZZY6: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy6"
+    )
+    FUZZY7: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy7"
+    )
+    FUZZY8: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy8"
+    )
+    FUZZY9: Optional[Union[StrictStr, "TokenPatternString"]] = Field(
+        None, alias="fuzzy9"
+    )
 
     class Config:
         extra = "forbid"
         allow_population_by_field_name = True  # allow alias and field name
 
     @validator("*", pre=True, each_item=True, allow_reuse=True)
     def raise_for_none(cls, v):
@@ -401,32 +418,55 @@
     # fmt: on
 
     class Config:
         extra = "forbid"
         arbitrary_types_allowed = True
 
 
+class ConfigSchemaDistillEmpty(BaseModel):
+    class Config:
+        extra = "forbid"
+
+
+class ConfigSchemaDistill(BaseModel):
+    # fmt: off
+    batcher: Batcher = Field(..., title="Batcher for the training data")
+    corpus: StrictStr = Field(..., title="Path in the config to the distillation data")
+    dropout: StrictFloat = Field(..., title="Dropout rate")
+    max_epochs: StrictInt = Field(..., title="Maximum number of epochs to distill for")
+    max_steps: StrictInt = Field(..., title="Maximum number of steps to distill for")
+    optimizer: Optimizer = Field(..., title="The optimizer to use")
+    student_to_teacher: Dict[str, str] = Field(..., title="Mapping from student to teacher pipe")
+    # fmt: on
+
+    class Config:
+        extra = "forbid"
+        arbitrary_types_allowed = True
+
+
 class ConfigSchema(BaseModel):
     training: ConfigSchemaTraining
     nlp: ConfigSchemaNlp
     pretraining: Union[ConfigSchemaPretrain, ConfigSchemaPretrainEmpty] = {}  # type: ignore[assignment]
     components: Dict[str, Dict[str, Any]]
     corpora: Dict[str, Reader]
     initialize: ConfigSchemaInit
+    distillation: Union[ConfigSchemaDistill, ConfigSchemaDistillEmpty] = {}  # type: ignore[assignment]
 
     class Config:
         extra = "allow"
         arbitrary_types_allowed = True
 
 
 CONFIG_SCHEMAS = {
     "nlp": ConfigSchemaNlp,
     "training": ConfigSchemaTraining,
     "pretraining": ConfigSchemaPretrain,
     "initialize": ConfigSchemaInit,
+    "distillation": ConfigSchemaDistill,
 }
 
 
 # Project config Schema
 
 
 class ProjectConfigAssetGitItem(BaseModel):
```

### Comparing `spacy-4.0.0.dev0/spacy/scorer.py` & `spacy-4.0.0.dev1/spacy/scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 class Scorer:
     """Compute evaluation scores."""
 
     def __init__(
         self,
         nlp: Optional["Language"] = None,
-        default_lang: str = "xx",
+        default_lang: str = "mul",
         default_pipeline: Iterable[str] = DEFAULT_PIPELINE,
         **cfg,
     ) -> None:
         """Initialize the Scorer.
 
         DOCS: https://spacy.io/api/scorer#init
         """
@@ -117,28 +117,38 @@
             self.nlp = nlp
         else:
             nlp = get_lang_class(default_lang)()
             for pipe in default_pipeline:
                 nlp.add_pipe(pipe)
             self.nlp = nlp
 
-    def score(self, examples: Iterable[Example]) -> Dict[str, Any]:
+    def score(
+        self, examples: Iterable[Example], *, per_component: bool = False
+    ) -> Dict[str, Any]:
         """Evaluate a list of Examples.
 
         examples (Iterable[Example]): The predicted annotations + correct annotations.
+        per_component (bool): Whether to return the scores keyed by component
+            name. Defaults to False.
         RETURNS (Dict): A dictionary of scores.
 
         DOCS: https://spacy.io/api/scorer#score
         """
         scores = {}
         if hasattr(self.nlp.tokenizer, "score"):
-            scores.update(self.nlp.tokenizer.score(examples, **self.cfg))  # type: ignore
+            if per_component:
+                scores["tokenizer"] = self.nlp.tokenizer.score(examples, **self.cfg)
+            else:
+                scores.update(self.nlp.tokenizer.score(examples, **self.cfg))  # type: ignore
         for name, component in self.nlp.pipeline:
             if hasattr(component, "score"):
-                scores.update(component.score(examples, **self.cfg))
+                if per_component:
+                    scores[name] = component.score(examples, **self.cfg)
+                else:
+                    scores.update(component.score(examples, **self.cfg))
         return scores
 
     @staticmethod
     def score_tokenization(examples: Iterable[Example], **cfg) -> Dict[str, Any]:
         """Returns accuracy and PRF scores for tokenization.
         * token_acc: # correct tokens / # gold tokens
         * token_p/r/f: PRF for token character spans
```

### Comparing `spacy-4.0.0.dev0/spacy/strings.pxd` & `spacy-4.0.0.dev1/spacy/strings.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/strings.pyi` & `spacy-4.0.0.dev1/spacy/strings.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, Iterable, Iterator, Union, Any, Tuple, overload
 from pathlib import Path
 
 class StringStore:
-    def __init__(self, strings: Optional[Iterable[str]]) -> None: ...
+    def __init__(self, strings: Optional[Iterable[str]] = None) -> None: ...
     @overload
     def __getitem__(self, string_or_hash: str) -> int: ...
     @overload
     def __getitem__(self, string_or_hash: int) -> str: ...
     def as_int(self, string_or_hash: Union[str, int]) -> int: ...
     def as_string(self, string_or_hash: Union[str, int]) -> str: ...
     def add(self, string: str) -> int: ...
```

### Comparing `spacy-4.0.0.dev0/spacy/strings.pyx` & `spacy-4.0.0.dev1/spacy/strings.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/structs.pxd` & `spacy-4.0.0.dev1/spacy/structs.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/symbols.pxd` & `spacy-4.0.0.dev1/spacy/symbols.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/symbols.pyx` & `spacy-4.0.0.dev1/spacy/symbols.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/conftest.py` & `spacy-4.0.0.dev1/spacy/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 # Fixtures for language tokenizers (languages sorted alphabetically)
 
 
 @pytest.fixture(scope="module")
 def tokenizer():
-    return get_lang_class("xx")().tokenizer
+    return get_lang_class("mul")().tokenizer
 
 
 @pytest.fixture(scope="session")
 def af_tokenizer():
     return get_lang_class("af")().tokenizer
 
 
@@ -239,16 +239,16 @@
 
 @pytest.fixture(scope="session")
 def id_tokenizer():
     return get_lang_class("id")().tokenizer
 
 
 @pytest.fixture(scope="session")
-def is_tokenizer():
-    return get_lang_class("is")().tokenizer
+def isl_tokenizer():
+    return get_lang_class("isl")().tokenizer
 
 
 @pytest.fixture(scope="session")
 def it_tokenizer():
     return get_lang_class("it")().tokenizer
 
 
@@ -333,14 +333,19 @@
 
 @pytest.fixture(scope="session")
 def ml_tokenizer():
     return get_lang_class("ml")().tokenizer
 
 
 @pytest.fixture(scope="session")
+def ms_tokenizer():
+    return get_lang_class("ms")().tokenizer
+
+
+@pytest.fixture(scope="session")
 def nb_tokenizer():
     return get_lang_class("nb")().tokenizer
 
 
 @pytest.fixture(scope="session")
 def ne_tokenizer():
     return get_lang_class("ne")().tokenizer
@@ -492,16 +497,16 @@
 @pytest.fixture(scope="session")
 def vi_tokenizer():
     pytest.importorskip("pyvi")
     return get_lang_class("vi")().tokenizer
 
 
 @pytest.fixture(scope="session")
-def xx_tokenizer():
-    return get_lang_class("xx")().tokenizer
+def mul_tokenizer():
+    return get_lang_class("mul")().tokenizer
 
 
 @pytest.fixture(scope="session")
 def yo_tokenizer():
     return get_lang_class("yo")().tokenizer
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_add_entities.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_add_entities.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_array.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_array.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_creation.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_creation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_doc_api.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_doc_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytest
 import warnings
 from thinc.api import NumpyOps, get_current_ops
 
 from spacy.attrs import DEP, ENT_IOB, ENT_TYPE, HEAD, IS_ALPHA, MORPH, POS
 from spacy.attrs import SENT_START, TAG
 from spacy.lang.en import English
-from spacy.lang.xx import MultiLanguage
+from spacy.lang.mul import MultiLanguage
 from spacy.language import Language
 from spacy.lexeme import Lexeme
 from spacy.tokens import Doc, Span, SpanGroup, Token
 from spacy.vocab import Vocab
 
 from .test_underscore import clean_underscore  # noqa: F401
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_graph.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_graph.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_json_doc_conversion.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_json_doc_conversion.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_morphanalysis.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_morphanalysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
     assert i_has[0].morph.key == i_has[0].morph.key
     assert i_has[0].morph.key != i_has[1].morph.key
 
 
 def test_morph_props(i_has):
     assert i_has[0].morph.get("PronType") == ["prs"]
     assert i_has[1].morph.get("PronType") == []
+    assert i_has[1].morph.get("AsdfType", ["asdf"]) == ["asdf"]
+    assert i_has[1].morph.get("AsdfType", default=["asdf", "qwer"]) == ["asdf", "qwer"]
 
 
 def test_morph_iter(i_has):
     assert set(i_has[0].morph) == set(["PronType=prs"])
     assert set(i_has[1].morph) == set(
         ["Number=sing", "Person=three", "Tense=pres", "VerbForm=fin"]
     )
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_pickle_doc.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_pickle_doc.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_retokenize_merge.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_retokenize_merge.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_retokenize_split.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_retokenize_split.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_span.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_span.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,14 +171,26 @@
         span.label = doc.vocab.strings["TEST"]
 
     # Span changes must be reflected in the span group
     assert group[0].start == 0
     assert group[0].label == doc.vocab.strings["TEST"]
 
 
+def test_char_span_attributes(doc):
+    label = "LABEL"
+    kb_id = "KB_ID"
+    span_id = "SPAN_ID"
+    span1 = doc.char_span(20, 45, label=label, kb_id=kb_id, span_id=span_id)
+    span2 = doc[1:].char_span(15, 40, label=label, kb_id=kb_id, span_id=span_id)
+    assert span1.text == span2.text
+    assert span1.label_ == span2.label_ == label
+    assert span1.kb_id_ == span2.kb_id_ == kb_id
+    assert span1.id_ == span2.id_ == span_id
+
+
 def test_spans_sent_spans(doc):
     sents = list(doc.sents)
     assert sents[0].start == 0
     assert sents[0].end == 5
     assert len(sents) == 3
     assert sum(len(sent) for sent in sents) == len(doc)
 
@@ -234,15 +246,14 @@
         (0, 1, "This is"),  # Beginning of the Doc. Part of a sentence
         (10, 14, "And a"),  # End of the Doc. Overlapping with 2 senteces
         (12, 14, "third."),  # End of the Doc. Full sentence
         (1, 1, "This is"),  # Empty Span
     ],
 )
 def test_spans_span_sent_user_hooks(doc, start, end, expected_sentence):
-
     # Doc-level sents hook
     def user_hook(doc):
         return [doc[ii : ii + 2] for ii in range(0, len(doc), 2)]
 
     doc.user_hooks["sents"] = user_hook
 
     # Make sure doc-level sents hook works
@@ -350,14 +361,22 @@
 
     # unsupported alignment mode
     with pytest.raises(ValueError):
         span2 = doc.char_span(
             span1.start_char + 1, span1.end_char, label="GPE", alignment_mode="unk"
         )
 
+    # Span.char_span + alignment mode "contract"
+    span2 = doc[0:2].char_span(
+        span1.start_char - 3, span1.end_char, label="GPE", alignment_mode="contract"
+    )
+    assert span1.start_char == span2.start_char
+    assert span1.end_char == span2.end_char
+    assert span2.label_ == "GPE"
+
 
 def test_span_to_array(doc):
     span = doc[1:-2]
     arr = span.to_array([ORTH, LENGTH])
     assert arr.shape == (len(span), 2)
     assert arr[0, 0] == span[0].orth
     assert arr[0, 1] == len(span[0])
@@ -631,15 +650,14 @@
         (9, 14, 2, 3),  # End of the Doc. Overlapping with 2 senteces
         (10, 14, 1, 2),  # End of the Doc. Full sentence
         (11, 14, 1, 2),  # End of the Doc. Partial sentence
         (0, 0, 1, 1),  # Empty Span
     ],
 )
 def test_span_sents(doc, start, end, expected_sentences, expected_sentences_with_hook):
-
     assert len(list(doc[start:end].sents)) == expected_sentences
 
     def user_hook(doc):
         return [doc[ii : ii + 2] for ii in range(0, len(doc), 2)]
 
     doc.user_hooks["sents"] = user_hook
 
@@ -683,7 +701,85 @@
     assert doc[1].ent_id_ == "ID1"
 
     # Span.ent_id is an alias of Span.id
     span.ent_id_ = "ID2"
     doc.ents = [span]
     assert doc.ents[0].ent_id_ == "ID2"
     assert doc[1].ent_id_ == "ID2"
+
+
+def test_span_start_end_sync(en_tokenizer):
+    doc = en_tokenizer("a bc def e fghij kl")
+    # can create and edit span starts/ends
+    span = doc[2:4]
+    span.start_char = 2
+    span.end = 5
+    assert span == doc[span.start : span.end]
+    assert span == doc.char_span(span.start_char, span.end_char)
+    # cannot set completely out of bounds starts/ends
+    with pytest.raises(IndexError):
+        span.start = -1
+    with pytest.raises(IndexError):
+        span.end = -1
+    with pytest.raises(IndexError):
+        span.start_char = len(doc.text) + 1
+    with pytest.raises(IndexError):
+        span.end = len(doc.text) + 1
+    # test all possible char starts/ends
+    span = doc[0 : len(doc)]
+    token_char_starts = [token.idx for token in doc]
+    token_char_ends = [token.idx + len(token.text) for token in doc]
+    for i in range(len(doc.text)):
+        if i not in token_char_starts:
+            with pytest.raises(ValueError):
+                span.start_char = i
+        else:
+            span.start_char = i
+    span = doc[0 : len(doc)]
+    for i in range(len(doc.text)):
+        if i not in token_char_ends:
+            with pytest.raises(ValueError):
+                span.end_char = i
+        else:
+            span.end_char = i
+    # start must be <= end
+    span = doc[1:3]
+    with pytest.raises(ValueError):
+        span.start = 4
+    with pytest.raises(ValueError):
+        span.end = 0
+    span = doc.char_span(2, 8)
+    with pytest.raises(ValueError):
+        span.start_char = 9
+    with pytest.raises(ValueError):
+        span.end_char = 1
+
+
+def test_for_partial_ent_sents():
+    """Spans may be associated with multiple sentences. These .sents should always be complete, not partial, sentences,
+    which this tests for.
+    """
+    doc = Doc(
+        English().vocab,
+        words=["Mahler's", "Symphony", "No.", "8", "was", "beautiful."],
+        sent_starts=[1, 0, 0, 1, 0, 0],
+    )
+    doc.set_ents([Span(doc, 1, 4, "WORK")])
+    # The specified entity is associated with both sentences in this doc, so we expect all sentences in the doc to be
+    # equal to the sentences referenced in ent.sents.
+    for doc_sent, ent_sent in zip(doc.sents, doc.ents[0].sents):
+        assert doc_sent == ent_sent
+
+
+def test_for_no_ent_sents():
+    """Span.sents() should set .sents correctly, even if Span in question is trailing and doesn't form a full
+    sentence.
+    """
+    doc = Doc(
+        English().vocab,
+        words=["This", "is", "a", "test.", "ENTITY"],
+        sent_starts=[1, 0, 0, 0, 1],
+    )
+    doc.set_ents([Span(doc, 4, 5, "WORK")])
+    sents = list(doc.ents[0].sents)
+    assert len(sents) == 1
+    assert str(sents[0]) == str(doc.ents[0].sent) == "ENTITY"
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_span_group.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_span_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,29 @@
     clone.attrs["key"] = "new_value"
     clone.append(Span(doc, 0, 6, "LABEL"))
     assert clone.name != span_group.name
     assert clone.attrs != span_group.attrs
     assert span_group.attrs["key"] == "value"
     assert list(span_group) != list(clone)
 
+    # can't copy if the character offsets don't align to tokens
+    doc2 = Doc(doc.vocab, words=[t.text + "x" for t in doc])
+    with pytest.raises(ValueError):
+        span_group.copy(doc=doc2)
+
+    # can copy with valid character offsets despite different tokenization
+    doc3 = doc.copy()
+    with doc3.retokenize() as retokenizer:
+        retokenizer.merge(doc3[0:2])
+        retokenizer.merge(doc3[3:6])
+    span_group = SpanGroup(doc, spans=[doc[0:6], doc[3:6]])
+    for span1, span2 in zip(span_group, span_group.copy(doc=doc3)):
+        assert span1.start_char == span2.start_char
+        assert span1.end_char == span2.end_char
+
 
 def test_span_group_set_item(doc, other_doc):
     span_group = doc.spans["SPANS"]
 
     index = 5
     span = span_group[index]
     span.label_ = "NEW LABEL"
@@ -251,7 +266,16 @@
 def test_span_group_typing(doc: Doc):
     """Tests whether typing of `SpanGroup` as `Iterable[Span]`-like object is accepted by mypy."""
     span_group: SpanGroup = doc.spans["SPANS"]
     spans: List[Span] = list(span_group)
     for i, span in enumerate(span_group):
         assert span == span_group[i] == spans[i]
     filter_spans(span_group)
+
+
+def test_span_group_init_doc(en_tokenizer):
+    """Test that all spans must come from the specified doc."""
+    doc1 = en_tokenizer("a b c")
+    doc2 = en_tokenizer("a b c")
+    span_group = SpanGroup(doc1, spans=[doc1[0:1], doc1[1:2]])
+    with pytest.raises(ValueError):
+        span_group = SpanGroup(doc1, spans=[doc1[0:1], doc2[1:2]])
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_token_api.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_token_api.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/doc/test_underscore.py` & `spacy-4.0.0.dev1/spacy/tests/doc/test_underscore.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/af/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/af/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/af/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/af/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/am/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/am/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ar/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ar/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ar/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ar/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/bn/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/bn/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ca/test_exception.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ca/test_exception.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ca/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ca/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/da/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/da/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/da/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/da/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/da/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/da/test_prefix_suffix_infix.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/da/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/da/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/de/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/de/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/de/test_parser.py` & `spacy-4.0.0.dev1/spacy/tests/lang/de/test_parser.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/de/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/de/test_prefix_suffix_infix.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/de/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/de/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/dsb/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/dsb/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/dsb/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/dsb/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/el/test_exception.py` & `spacy-4.0.0.dev1/spacy/tests/lang/el/test_exception.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/el/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/el/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_customized_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_customized_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_indices.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_indices.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_parser.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_parser.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_prefix_suffix_infix.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_punct.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_punct.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_sbd.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_sbd.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/en/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/en/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/es/test_exception.py` & `spacy-4.0.0.dev1/spacy/tests/lang/es/test_exception.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/es/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/es/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/es/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/es/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/et/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/et/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/et/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/et/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fi/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fi/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fi/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fi/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fi/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fi/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fr/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fr/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fr/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fr/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fr/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fr/test_prefix_suffix_infix.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/fr/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/fr/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ga/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ga/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/grc/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/grc/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/grc/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/grc/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/gu/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/gu/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/he/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/he/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hi/test_lex_attrs.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hi/test_lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hr/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hr/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hr/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hr/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hsb/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hsb/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hsb/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hsb/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hu/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hu/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/hy/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/hy/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/id/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/id/test_prefix_suffix_infix.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/is/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/isl/test_text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
 
 
-def test_long_text(is_tokenizer):
+def test_long_text(isl_tokenizer):
     # Excerpt: European Convention on Human Rights
     text = """
 hafa í huga, að yfirlýsing þessi hefur það markmið að tryggja
 almenna og raunhæfa viðurkenningu og vernd þeirra réttinda,
 sem þar er lýst;
 hafa í huga, að markmið Evrópuráðs er að koma á nánari einingu
 aðildarríkjanna og að ein af leiðunum að því marki er sú, að
 mannréttindi og mannfrelsi séu í heiðri höfð og efld;
 lýsa á ný eindreginni trú sinni á það mannfrelsi, sem er undirstaða
 réttlætis og friðar í heiminum og best er tryggt, annars vegar með
 virku, lýðræðislegu stjórnarfari og, hins vegar, almennum skilningi
 og varðveislu þeirra mannréttinda, sem eru grundvöllur frelsisins;
 """
-    tokens = is_tokenizer(text)
+    tokens = isl_tokenizer(text)
     assert len(tokens) == 120
 
 
 @pytest.mark.xfail
-def test_ordinal_number(is_tokenizer):
+def test_ordinal_number(isl_tokenizer):
     text = "10. desember 1948"
-    tokens = is_tokenizer(text)
+    tokens = isl_tokenizer(text)
     assert len(tokens) == 3
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/is/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/isl/test_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-IS_BASIC_TOKENIZATION_TESTS = [
+ISL_BASIC_TOKENIZATION_TESTS = [
     (
         "Enginn maður skal sæta pyndingum eða ómannlegri eða "
         "vanvirðandi meðferð eða refsingu. ",
         [
             "Enginn",
             "maður",
             "skal",
@@ -19,12 +19,12 @@
             "refsingu",
             ".",
         ],
     ),
 ]
 
 
-@pytest.mark.parametrize("text,expected_tokens", IS_BASIC_TOKENIZATION_TESTS)
-def test_is_tokenizer_basic(is_tokenizer, text, expected_tokens):
-    tokens = is_tokenizer(text)
+@pytest.mark.parametrize("text,expected_tokens", ISL_BASIC_TOKENIZATION_TESTS)
+def test_isl_tokenizer_basic(isl_tokenizer, text, expected_tokens):
+    tokens = isl_tokenizer(text)
     token_list = [token.text for token in tokens if not token.is_space]
     assert expected_tokens == token_list
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/it/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/it/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ja/test_lemmatization.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ja/test_lemmatization.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ja/test_serialize.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ja/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ja/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ja/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ko/test_lemmatization.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ko/test_lemmatization.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ko/test_serialize.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ko/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ko/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ko/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ky/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ky/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/la/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/la/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/lb/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/lb/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/lb/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/lb/test_prefix_suffix_infix.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/lb/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/lb/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/lt/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/lt/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/lv/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/lv/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/lv/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/lv/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/mk/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/mk/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ml/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ml/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/nb/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/nb/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ne/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ne/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/nl/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/nl/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/nl/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/nl/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/pl/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/pl/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/pl/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/pl/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/pt/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/pt/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ro/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ro/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ru/test_lemmatizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ru/test_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ru/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ru/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sa/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sa/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sk/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sk/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sl/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sl/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sl/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sl/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sq/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sq/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sq/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sq/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sr/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sr/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sv/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sv/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sv/test_lex_attrs.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sv/test_lex_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sv/test_noun_chunks.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sv/test_noun_chunks.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sv/test_prefix_suffix_infix.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sv/test_prefix_suffix_infix.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,7 +28,14 @@
     assert tokens[2].text == text.split(",")[1]
 
 
 @pytest.mark.parametrize("text", ["svart...Gul", "svart...gul"])
 def test_tokenizer_splits_ellipsis_infix(sv_tokenizer, text):
     tokens = sv_tokenizer(text)
     assert len(tokens) == 3
+
+
+@pytest.mark.issue(12311)
+@pytest.mark.parametrize("text", ["99:e", "c:a", "EU:s", "Maj:t"])
+def test_sv_tokenizer_handles_colon(sv_tokenizer, text):
+    tokens = sv_tokenizer(text)
+    assert len(tokens) == 1
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sv/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sv/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/sv/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/sv/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ta/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ta/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ta/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ta/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/test_attrs.py` & `spacy-4.0.0.dev1/spacy/tests/lang/test_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/test_initialize.py` & `spacy-4.0.0.dev1/spacy/tests/lang/test_initialize.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 
 # fmt: off
 # Only include languages with no external dependencies
 # excluded: ja, ko, th, vi, zh
 LANGUAGES = ["af", "am", "ar", "az", "bg", "bn", "ca", "cs", "da", "de", "el",
              "en", "es", "et", "eu", "fa", "fi", "fr", "ga", "gu", "he", "hi",
-             "hr", "hu", "hy", "id", "is", "it", "kn", "ky", "lb", "lt", "lv",
-             "mk", "ml", "mr", "nb", "ne", "nl", "pl", "pt", "ro", "ru", "sa",
+             "hr", "hu", "hy", "id", "isl", "it", "kn", "ky", "lb", "lt", "lv",
+             "mk", "ml", "mr", "mul", "nb", "ne", "nl", "pl", "pt", "ro", "ru", "sa",
              "si", "sk", "sl", "sq", "sr", "sv", "ta", "te", "ti", "tl", "tn",
-             "tr", "tt", "uk", "ur", "xx", "yo"]
+             "tr", "tt", "uk", "ur", "yo"]
 # fmt: on
 
 
 @pytest.mark.parametrize("lang", LANGUAGES)
 def test_lang_initialize(lang, capfd):
     """Test that languages can be initialized."""
     nlp = get_lang_class(lang)()
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/test_lemmatizers.py` & `spacy-4.0.0.dev1/spacy/tests/lang/test_lemmatizers.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/th/test_serialize.py` & `spacy-4.0.0.dev1/spacy/tests/lang/th/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/ti/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/ti/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/tl/test_punct.py` & `spacy-4.0.0.dev1/spacy/tests/lang/tl/test_punct.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/tl/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/tl/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/tr/test_parser.py` & `spacy-4.0.0.dev1/spacy/tests/lang/tr/test_parser.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/tr/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/tr/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/tr/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/tr/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/tt/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/tt/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/uk/test_lemmatizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/uk/test_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/uk/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/uk/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/vi/test_serialize.py` & `spacy-4.0.0.dev1/spacy/tests/lang/vi/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/vi/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/vi/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/xx/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/mul/test_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 
-def test_long_text(xx_tokenizer):
+def test_long_text(mul_tokenizer):
     # Excerpt: Text in Skolt Sami taken from https://www.samediggi.fi
     text = """
 Säʹmmla lie Euroopp unioon oʹdinakai alggmeer. Säʹmmlai alggmeerstatus lij raʹvvjum Lääʹddjânnam vuâđđlääʹjjest.  
 Alggmeer kriteeʹr vuâđđâʹvve meeraikõskksaž tuâjjorganisaatio, ILO, suåppmõʹšše nââmar 169. 
 Suåppmõõžž mieʹldd jiõččvälddsaž jânnmin jälsteei meeraid ââʹnet alggmeeran, 
 ko sij puõlvvâʹvve naroodâst, kååʹtt jânnam välddmõõžž leʹbe aazztummuž leʹbe ânnʼjõž riikkraaʹji šõddâm ääiʹj jälste 
 jânnmest leʹbe tõn mäddtiõđlaž vuuʹdest, koozz jânnam kooll. Alggmeer ij leäkku mieʹrreei sââʹjest jiiʹjjes jälstemvuuʹdest. 
@@ -16,9 +16,9 @@
 Säʹmmlai statuuzz ǩeeʹrjteš Lääʹddjânnam vuâđđläkka eeʹjj 1995. Säʹmmlain alggmeeran lij vuõiggâdvuõtt tuõʹllʼjed da 
 ooudâsviikkâd ǩiõlâz da kulttuurâz di tõõzz kuulli ääʹrbvuâlaž jieʹllemvueʹjjeez. Sääʹmǩiõl ââʹnnmest veʹrǧǧniiʹǩǩi 
 åʹrnn lij šiõttuum jiiʹjjes lääʹǩǩ. Säʹmmlain lij leämmaž eeʹjjest 1996 vueʹljeeʹl dommvuuʹdsteez ǩiõlâz da kulttuurâz kuõskki 
 vuâđđlääʹjj meâldlaž jiõččvaaldâšm. Säʹmmlai jiõččvaldšma kuulli tuâjaid håidd säʹmmlai vaalin vaʹlljääm parlameʹntt, 
 Sääʹmteʹǧǧ.
 """
 
-    tokens = xx_tokenizer(text)
+    tokens = mul_tokenizer(text)
     assert len(tokens) == 179
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/xx/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/mul/test_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-XX_BASIC_TOKENIZATION_TESTS = [
+MUL_BASIC_TOKENIZATION_TESTS = [
     (
         "Lääʹddjânnmest lie nuʹtt 10 000 säʹmmliʹžžed. Seeʹst pâʹjjel",
         [
             "Lääʹddjânnmest",
             "lie",
             "nuʹtt",
             "10",
@@ -14,12 +14,12 @@
             "Seeʹst",
             "pâʹjjel",
         ],
     ),
 ]
 
 
-@pytest.mark.parametrize("text,expected_tokens", XX_BASIC_TOKENIZATION_TESTS)
-def test_xx_tokenizer_basic(xx_tokenizer, text, expected_tokens):
-    tokens = xx_tokenizer(text)
+@pytest.mark.parametrize("text,expected_tokens", MUL_BASIC_TOKENIZATION_TESTS)
+def test_mul_tokenizer_basic(mul_tokenizer, text, expected_tokens):
+    tokens = mul_tokenizer(text)
     token_list = [token.text for token in tokens if not token.is_space]
     assert expected_tokens == token_list
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/yo/test_text.py` & `spacy-4.0.0.dev1/spacy/tests/lang/yo/test_text.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/zh/test_serialize.py` & `spacy-4.0.0.dev1/spacy/tests/lang/zh/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/lang/zh/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/lang/zh/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/matcher/test_dependency_matcher.py` & `spacy-4.0.0.dev1/spacy/tests/matcher/test_dependency_matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -312,24 +312,40 @@
         ("brown", "brown", "$-", 0),
         ("the", "brown", "$++", 1),
         ("brown", "the", "$++", 0),
         ("brown", "brown", "$++", 0),
         ("the", "brown", "$--", 0),
         ("brown", "the", "$--", 1),
         ("brown", "brown", "$--", 0),
+        ("over", "jumped", "<+", 0),
+        ("quick", "fox", "<+", 0),
+        ("the", "quick", "<+", 0),
+        ("brown", "fox", "<+", 1),
         ("quick", "fox", "<++", 1),
         ("quick", "over", "<++", 0),
         ("over", "jumped", "<++", 0),
         ("the", "fox", "<++", 2),
+        ("brown", "fox", "<-", 0),
+        ("fox", "over", "<-", 0),
+        ("the", "over", "<-", 0),
+        ("over", "jumped", "<-", 1),
         ("brown", "fox", "<--", 0),
         ("fox", "jumped", "<--", 0),
         ("fox", "over", "<--", 1),
+        ("fox", "brown", ">+", 0),
+        ("over", "fox", ">+", 0),
+        ("over", "the", ">+", 0),
+        ("jumped", "over", ">+", 1),
         ("jumped", "over", ">++", 1),
         ("fox", "lazy", ">++", 0),
         ("over", "the", ">++", 0),
+        ("jumped", "over", ">-", 0),
+        ("fox", "quick", ">-", 0),
+        ("brown", "quick", ">-", 0),
+        ("fox", "brown", ">-", 1),
         ("brown", "fox", ">--", 0),
         ("fox", "brown", ">--", 1),
         ("jumped", "fox", ">--", 1),
         ("fox", "the", ">--", 2),
     ],
 )
 def test_dependency_matcher_ops(en_vocab, doc, left, right, op, num_matches):
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/matcher/test_levenshtein.py` & `spacy-4.0.0.dev1/spacy/tests/matcher/test_levenshtein.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/matcher/test_matcher_api.py` & `spacy-4.0.0.dev1/spacy/tests/matcher/test_matcher_api.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/matcher/test_matcher_logic.py` & `spacy-4.0.0.dev1/spacy/tests/matcher/test_matcher_logic.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/matcher/test_pattern_validation.py` & `spacy-4.0.0.dev1/spacy/tests/matcher/test_pattern_validation.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/matcher/test_phrase_matcher.py` & `spacy-4.0.0.dev1/spacy/tests/matcher/test_phrase_matcher.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/morphology/test_morph_converters.py` & `spacy-4.0.0.dev1/spacy/tests/morphology/test_morph_converters.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/morphology/test_morph_features.py` & `spacy-4.0.0.dev1/spacy/tests/morphology/test_morph_features.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/morphology/test_morph_pickle.py` & `spacy-4.0.0.dev1/spacy/tests/morphology/test_morph_pickle.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/package/requirements.txt` & `spacy-4.0.0.dev1/spacy/tests/package/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # Our libraries
-spacy-legacy>=3.0.11,<3.1.0
+spacy-legacy>=4.0.0.dev0,<4.1.0
 spacy-loggers>=1.0.0,<2.0.0
 cymem>=2.0.2,<2.1.0
 preshed>=3.0.2,<3.1.0
 thinc>=9.0.0.dev2,<9.1.0
 ml_datasets>=0.2.0,<0.3.0
 murmurhash>=0.28.0,<1.1.0
 wasabi>=0.9.1,<1.2.0
 srsly>=2.4.3,<3.0.0
 catalogue>=2.0.6,<2.1.0
-typer>=0.3.0,<0.8.0
+typer>=0.3.0,<0.10.0
 pathy>=0.10.0
 smart-open>=5.2.1,<7.0.0
 # Third party dependencies
 numpy>=1.15.0
 requests>=2.13.0,<3.0.0
 tqdm>=4.38.0,<5.0.0
 pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
 jinja2
 langcodes>=3.2.0,<4.0.0
 # Official Python utilities
 setuptools
 packaging>=20.0
-typing_extensions>=3.7.4.1,<4.2.0; python_version < "3.8"
 # Development dependencies
 pre-commit>=2.13.0
 cython>=0.25,<3.0
 pytest>=5.2.0,!=7.1.0
 pytest-timeout>=1.3.0,<2.0.0
 mock>=2.0.0,<3.0.0
 flake8>=3.8.0,<6.0.0
 hypothesis>=3.27.0,<7.0.0
-mypy>=0.990,<0.1000; platform_machine != "aarch64" and python_version >= "3.7"
-types-dataclasses>=0.1.3; python_version < "3.7"
+mypy>=0.990,<1.1.0; platform_machine != "aarch64"
 types-mock>=0.1.1
 types-setuptools>=57.0.0
 types-requests
 types-setuptools>=57.0.0
-black>=22.0,<23.0
+black==22.3.0
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/package/setup.cfg` & `spacy-4.0.0.dev1/spacy/tests/package/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -13,102 +13,107 @@
     Intended Audience :: Science/Research
     License :: OSI Approved :: MIT License
     Operating System :: POSIX :: Linux
     Operating System :: MacOS :: MacOS X
     Operating System :: Microsoft :: Windows
     Programming Language :: Cython
     Programming Language :: Python :: 3
-    Programming Language :: Python :: 3.6
-    Programming Language :: Python :: 3.7
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     Programming Language :: Python :: 3.10
     Programming Language :: Python :: 3.11
     Topic :: Scientific/Engineering
 project_urls =
     Release notes = https://github.com/explosion/spaCy/releases
     Source = https://github.com/explosion/spaCy
 
 [options]
 zip_safe = false
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
+setup_requires =
+    cython>=0.25,<3.0
+    numpy>=1.15.0
+    # We also need our Cython packages here to compile against
+    cymem>=2.0.2,<2.1.0
+    preshed>=3.0.2,<3.1.0
+    murmurhash>=0.28.0,<1.1.0
+    thinc>=9.0.0.dev2,<9.1.0
 install_requires =
     # Our libraries
-    spacy-legacy>=3.0.11,<3.1.0
+    spacy-legacy>=4.0.0.dev0,<4.1.0
     spacy-loggers>=1.0.0,<2.0.0
     murmurhash>=0.28.0,<1.1.0
     cymem>=2.0.2,<2.1.0
     preshed>=3.0.2,<3.1.0
     thinc>=9.0.0.dev2,<9.1.0
     wasabi>=0.9.1,<1.2.0
     srsly>=2.4.3,<3.0.0
     catalogue>=2.0.6,<2.1.0
     # Third-party dependencies
-    typer>=0.3.0,<0.8.0
+    typer>=0.3.0,<0.10.0
     pathy>=0.10.0
     smart-open>=5.2.1,<7.0.0
     tqdm>=4.38.0,<5.0.0
     numpy>=1.15.0
     requests>=2.13.0,<3.0.0
     pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
     jinja2
     # Official Python utilities
     setuptools
     packaging>=20.0
-    typing_extensions>=3.7.4,<4.2.0; python_version < "3.8"
     langcodes>=3.2.0,<4.0.0
 
 [options.entry_points]
 console_scripts =
     spacy = spacy.cli:setup_cli
 
 [options.extras_require]
 lookups =
     spacy_lookups_data>=1.0.3,<1.1.0
 transformers =
     spacy_transformers>=1.1.2,<1.3.0
 ray =
     spacy_ray>=0.1.0,<1.0.0
 cuda =
-    cupy>=5.0.0b4,<12.0.0
+    cupy>=5.0.0b4,<13.0.0
 cuda80 =
-    cupy-cuda80>=5.0.0b4,<12.0.0
+    cupy-cuda80>=5.0.0b4,<13.0.0
 cuda90 =
-    cupy-cuda90>=5.0.0b4,<12.0.0
+    cupy-cuda90>=5.0.0b4,<13.0.0
 cuda91 =
-    cupy-cuda91>=5.0.0b4,<12.0.0
+    cupy-cuda91>=5.0.0b4,<13.0.0
 cuda92 =
-    cupy-cuda92>=5.0.0b4,<12.0.0
+    cupy-cuda92>=5.0.0b4,<13.0.0
 cuda100 =
-    cupy-cuda100>=5.0.0b4,<12.0.0
+    cupy-cuda100>=5.0.0b4,<13.0.0
 cuda101 =
-    cupy-cuda101>=5.0.0b4,<12.0.0
+    cupy-cuda101>=5.0.0b4,<13.0.0
 cuda102 =
-    cupy-cuda102>=5.0.0b4,<12.0.0
+    cupy-cuda102>=5.0.0b4,<13.0.0
 cuda110 =
-    cupy-cuda110>=5.0.0b4,<12.0.0
+    cupy-cuda110>=5.0.0b4,<13.0.0
 cuda111 =
-    cupy-cuda111>=5.0.0b4,<12.0.0
+    cupy-cuda111>=5.0.0b4,<13.0.0
 cuda112 =
-    cupy-cuda112>=5.0.0b4,<12.0.0
+    cupy-cuda112>=5.0.0b4,<13.0.0
 cuda113 =
-    cupy-cuda113>=5.0.0b4,<12.0.0
+    cupy-cuda113>=5.0.0b4,<13.0.0
 cuda114 =
-    cupy-cuda114>=5.0.0b4,<12.0.0
+    cupy-cuda114>=5.0.0b4,<13.0.0
 cuda115 =
-    cupy-cuda115>=5.0.0b4,<12.0.0
+    cupy-cuda115>=5.0.0b4,<13.0.0
 cuda116 =
-    cupy-cuda116>=5.0.0b4,<12.0.0
+    cupy-cuda116>=5.0.0b4,<13.0.0
 cuda117 =
-    cupy-cuda117>=5.0.0b4,<12.0.0
+    cupy-cuda117>=5.0.0b4,<13.0.0
 cuda11x =
-    cupy-cuda11x>=11.0.0,<12.0.0
+    cupy-cuda11x>=11.0.0,<13.0.0
 cuda-autodetect =
-    cupy-wheel>=11.0.0,<12.0.0
+    cupy-wheel>=11.0.0,<13.0.0
 apple =
     thinc-apple-ops>=0.1.0.dev0,<1.0.0
 # Language tokenizers with external dependencies
 ja =
     sudachipy>=0.5.2,!=0.6.1
     sudachidict_core>=20211220
 ko =
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/package/test_requirements.py` & `spacy-4.0.0.dev1/spacy/tests/package/test_requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from pathlib import Path
 
 
 def test_build_dependencies():
     # Check that library requirements are pinned exactly the same across different setup files.
     libs_ignore_requirements = [
-        "cython",
         "pytest",
         "pytest-timeout",
         "mock",
         "flake8",
         "hypothesis",
         "pre-commit",
         "black",
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/_search.pyx` & `spacy-4.0.0.dev1/spacy/tests/parser/_search.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_add_label.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_add_label.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_arc_eager_oracle.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_arc_eager_oracle.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_ner.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from spacy.attrs import ENT_IOB
 from spacy import util, registry
 from spacy.lang.en import English
 from spacy.lang.it import Italian
 from spacy.language import Language
 from spacy.lookups import Lookups
+from spacy.pipeline import EntityRecognizer
+from spacy.pipeline.ner import DEFAULT_NER_MODEL
 from spacy.pipeline._parser_internals.ner import BiluoPushDown
 from spacy.training import Example, iob_to_biluo, split_bilu_label
 from spacy.tokens import Doc, Span
 from spacy.vocab import Vocab
 from thinc.api import fix_random_seed
 import logging
 
 from ..util import make_tempdir
-from ...pipeline import EntityRecognizer
-from ...pipeline.ner import DEFAULT_NER_MODEL
 
 TRAIN_DATA = [
     ("Who is Shaka Khan?", {"entities": [(7, 17, "PERSON")]}),
     ("I like London and Berlin.", {"entities": [(7, 13, "LOC"), (18, 24, "LOC")]}),
 ]
 
 
@@ -619,15 +619,17 @@
 
 def test_is_distillable():
     nlp = English()
     ner = nlp.add_pipe("ner")
     assert ner.is_distillable
 
 
-def test_distill():
+@pytest.mark.slow
+@pytest.mark.parametrize("max_moves", [0, 1, 5, 100])
+def test_distill(max_moves):
     teacher = English()
     teacher_ner = teacher.add_pipe("ner")
     train_examples = []
     for text, annotations in TRAIN_DATA:
         train_examples.append(Example.from_dict(teacher.make_doc(text), annotations))
         for ent in annotations.get("entities"):
             teacher_ner.add_label(ent[2])
@@ -637,14 +639,15 @@
     for i in range(50):
         losses = {}
         teacher.update(train_examples, sgd=optimizer, losses=losses)
     assert losses["ner"] < 0.00001
 
     student = English()
     student_ner = student.add_pipe("ner")
+    student_ner.cfg["update_with_oracle_cut_size"] = max_moves
     student_ner.initialize(
         get_examples=lambda: train_examples, labels=teacher_ner.label_data
     )
 
     distill_examples = [
         Example.from_dict(teacher.make_doc(t[0]), {}) for t in TRAIN_DATA
     ]
@@ -770,17 +773,17 @@
     ner = nlp.add_pipe("beam_ner", config=config)
     train_text = "Who is Shaka Khan?"
     neg_doc = nlp.make_doc(train_text)
     ner.add_label("PERSON")
     ner.add_label("ORG")
     example = Example.from_dict(neg_doc, {"entities": [(7, 17, "PERSON")]})
     example.reference.spans[neg_key] = [
-        Span(neg_doc, 2, 4, "ORG"),
-        Span(neg_doc, 2, 3, "PERSON"),
-        Span(neg_doc, 1, 4, "PERSON"),
+        Span(example.reference, 2, 4, "ORG"),
+        Span(example.reference, 2, 3, "PERSON"),
+        Span(example.reference, 1, 4, "PERSON"),
     ]
 
     optimizer = nlp.initialize()
     for i in range(2):
         losses = {}
         nlp.update([example], sgd=optimizer, losses=losses)
 
@@ -797,15 +800,15 @@
     }
     ner = nlp.add_pipe("beam_ner", config=config)
     train_text = "Who is Shaka Khan?"
     neg_doc = nlp.make_doc(train_text)
     ner.add_label("PERSON")
     ner.add_label("LOC")
     example = Example.from_dict(neg_doc, {"entities": [(7, 17, "PERSON")]})
-    example.reference.spans[neg_key] = [Span(neg_doc, 2, 4, "PERSON")]
+    example.reference.spans[neg_key] = [Span(example.reference, 2, 4, "PERSON")]
     assert len(example.reference.ents) == 1
     assert example.reference.ents[0].text == "Shaka Khan"
     assert example.reference.ents[0].label_ == "PERSON"
     assert len(example.reference.spans[neg_key]) == 1
     assert example.reference.spans[neg_key][0].text == "Shaka Khan"
     assert example.reference.spans[neg_key][0].label_ == "PERSON"
 
@@ -830,15 +833,15 @@
     # fmt: off
     tokens = ['FEDERAL', 'NATIONAL', 'MORTGAGE', 'ASSOCIATION', '(', 'Fannie', 'Mae', '):', 'Posted', 'yields', 'on', '30', 'year', 'mortgage', 'commitments', 'for', 'delivery', 'within', '30', 'days', '(', 'priced', 'at', 'par', ')', '9.75', '%', ',', 'standard', 'conventional', 'fixed', '-', 'rate', 'mortgages', ';', '8.70', '%', ',', '6/2', 'rate', 'capped', 'one', '-', 'year', 'adjustable', 'rate', 'mortgages', '.', 'Source', ':', 'Telerate', 'Systems', 'Inc.']
     iob = ['B-ORG', 'I-ORG', 'I-ORG', 'L-ORG', 'O', 'B-ORG', 'L-ORG', 'O', 'O', 'O', 'O', 'B-DATE', 'L-DATE', 'O', 'O', 'O', 'O', 'O', 'B-DATE', 'L-DATE', 'O', 'O', 'O', 'O', 'O', 'B-PERCENT', 'L-PERCENT', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'B-PERCENT', 'L-PERCENT', 'O', 'U-CARDINAL', 'O', 'O', 'B-DATE', 'I-DATE', 'L-DATE', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O', 'O']
     # fmt: on
 
     doc = Doc(nlp.vocab, words=tokens)
     example = Example.from_dict(doc, {"ner": iob})
-    neg_span = Span(doc, 50, 53, "ORG")
+    neg_span = Span(example.reference, 50, 53, "ORG")
     example.reference.spans[neg_key] = [neg_span]
 
     optimizer = nlp.initialize()
 
     for i in range(5):
         losses = {}
         nlp.update([example], sgd=optimizer, losses=losses)
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_neural_parser.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_neural_parser.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_nn_beam.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_nn_beam.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_nonproj.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_nonproj.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_parse.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 
 from spacy import registry, util
 from spacy.attrs import DEP, NORM
 from spacy.lang.en import English
 from spacy.training import Example
 from spacy.tokens import Doc
 from spacy.vocab import Vocab
-from spacy import util, registry
+from spacy.pipeline import DependencyParser
+from spacy.pipeline.dep_parser import DEFAULT_PARSER_MODEL
+from spacy.pipeline.tok2vec import DEFAULT_TOK2VEC_MODEL
 from thinc.api import fix_random_seed
 
-from ...pipeline import DependencyParser
-from ...pipeline.dep_parser import DEFAULT_PARSER_MODEL
 from ..util import apply_transition_sequence, make_tempdir
-from ...pipeline.tok2vec import DEFAULT_TOK2VEC_MODEL
 
 TRAIN_DATA = [
     (
         "They trade mortgage-backed securities.",
         {
             "heads": [1, 1, 4, 4, 5, 1, 1],
             "deps": ["nsubj", "ROOT", "compound", "punct", "nmod", "dobj", "punct"],
@@ -206,15 +205,15 @@
     active_states = states
 
     for step_actions in actions:
         active_states = moves.apply_actions(active_states, step_actions)
 
     assert len(active_states) == 0
 
-    for (state, doc) in zip(states, docs):
+    for state, doc in zip(states, docs):
         moves.set_annotations(state, doc)
 
     assert docs[0][0].head.i == 1
     assert docs[0][0].dep_ == "nsubj"
     assert docs[0][1].head.i == 1
     assert docs[0][1].dep_ == "ROOT"
     assert docs[0][2].head.i == 1
@@ -459,15 +458,17 @@
 
 def test_is_distillable():
     nlp = English()
     parser = nlp.add_pipe("parser")
     assert parser.is_distillable
 
 
-def test_distill():
+@pytest.mark.slow
+@pytest.mark.parametrize("max_moves", [0, 1, 5, 100])
+def test_distill(max_moves):
     teacher = English()
     teacher_parser = teacher.add_pipe("parser")
     train_examples = []
     for text, annotations in TRAIN_DATA:
         train_examples.append(Example.from_dict(teacher.make_doc(text), annotations))
         for dep in annotations.get("deps", []):
             teacher_parser.add_label(dep)
@@ -477,14 +478,15 @@
     for i in range(200):
         losses = {}
         teacher.update(train_examples, sgd=optimizer, losses=losses)
     assert losses["parser"] < 0.0001
 
     student = English()
     student_parser = student.add_pipe("parser")
+    student_parser.cfg["update_with_oracle_cut_size"] = max_moves
     student_parser.initialize(
         get_examples=lambda: train_examples, labels=teacher_parser.label_data
     )
 
     distill_examples = [
         Example.from_dict(teacher.make_doc(t[0]), {}) for t in TRAIN_DATA
     ]
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_parse_navigate.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_parse_navigate.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_preset_sbd.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_preset_sbd.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_space_attachment.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_space_attachment.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/parser/test_state.py` & `spacy-4.0.0.dev1/spacy/tests/parser/test_state.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_analysis.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_analysis.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_annotates_on_update.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_annotates_on_update.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,28 +50,36 @@
 def test_annotates_on_update():
     # The custom component checks for sentence annotation
     @Language.factory("assert_sents", default_config={})
     def assert_sents(nlp, name):
         return AssertSents(name)
 
     class AssertSents:
+        model = None
+        is_trainable = True
+
         def __init__(self, name, **cfg):
             self.name = name
-            pass
 
         def __call__(self, doc):
             if not doc.has_annotation("SENT_START"):
                 raise ValueError("No sents")
             return doc
 
         def update(self, examples, *, drop=0.0, sgd=None, losses=None):
+            losses.setdefault(self.name, 0.0)
+
             for example in examples:
                 if not example.predicted.has_annotation("SENT_START"):
                     raise ValueError("No sents")
-            return {}
+
+            return losses
+
+        def finish_update(self, sgd=None):
+            pass
 
     nlp = English()
     nlp.add_pipe("sentencizer")
     nlp.add_pipe("assert_sents")
 
     # When the pipeline runs, annotations are set
     nlp("This is a sentence.")
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_attributeruler.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_attributeruler.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_edit_tree_lemmatizer.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_edit_tree_lemmatizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,36 +99,38 @@
                 "suffix_tree": 4294967295,
             },
         ],
         "labels": (1, 3, 4, 6),
     }
 
 
-def test_no_data():
+@pytest.mark.parametrize("top_k", (1, 5, 30))
+def test_no_data(top_k):
     # Test that the lemmatizer provides a nice error when there's no tagging data / labels
     TEXTCAT_DATA = [
         ("I'm so happy.", {"cats": {"POSITIVE": 1.0, "NEGATIVE": 0.0}}),
         ("I'm so angry", {"cats": {"POSITIVE": 0.0, "NEGATIVE": 1.0}}),
     ]
     nlp = English()
-    nlp.add_pipe("trainable_lemmatizer")
+    nlp.add_pipe("trainable_lemmatizer", config={"top_k": top_k})
     nlp.add_pipe("textcat")
 
     train_examples = []
     for t in TEXTCAT_DATA:
         train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
 
     with pytest.raises(ValueError):
         nlp.initialize(get_examples=lambda: train_examples)
 
 
-def test_incomplete_data():
+@pytest.mark.parametrize("top_k", (1, 5, 30))
+def test_incomplete_data(top_k):
     # Test that the lemmatizer works with incomplete information
     nlp = English()
-    lemmatizer = nlp.add_pipe("trainable_lemmatizer")
+    lemmatizer = nlp.add_pipe("trainable_lemmatizer", config={"top_k": top_k})
     lemmatizer.min_tree_freq = 1
     train_examples = []
     for t in PARTIAL_DATA:
         train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
     optimizer = nlp.initialize(get_examples=lambda: train_examples)
     for i in range(50):
         losses = {}
@@ -137,18 +139,33 @@
 
     # test the trained model
     test_text = "She likes blue eggs"
     doc = nlp(test_text)
     assert doc[1].lemma_ == "like"
     assert doc[2].lemma_ == "blue"
 
+    # Check that incomplete annotations are ignored.
+    scores, _ = lemmatizer.model([eg.predicted for eg in train_examples], is_train=True)
+    _, dX = lemmatizer.get_loss(train_examples, scores)
+    xp = lemmatizer.model.ops.xp
+
+    # Missing annotations.
+    assert xp.count_nonzero(dX[0][0]) == 0
+    assert xp.count_nonzero(dX[0][3]) == 0
+    assert xp.count_nonzero(dX[1][0]) == 0
+    assert xp.count_nonzero(dX[1][3]) == 0
 
-def test_overfitting_IO():
+    # Misaligned annotations.
+    assert xp.count_nonzero(dX[1][1]) == 0
+
+
+@pytest.mark.parametrize("top_k", (1, 5, 30))
+def test_overfitting_IO(top_k):
     nlp = English()
-    lemmatizer = nlp.add_pipe("trainable_lemmatizer")
+    lemmatizer = nlp.add_pipe("trainable_lemmatizer", config={"top_k": top_k})
     lemmatizer.min_tree_freq = 1
     train_examples = []
     for t in TRAIN_DATA:
         train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
 
     optimizer = nlp.initialize(get_examples=lambda: train_examples)
 
@@ -173,15 +190,15 @@
         assert doc2[1].lemma_ == "like"
         assert doc2[2].lemma_ == "blue"
         assert doc2[3].lemma_ == "egg"
 
     # Check model after a {to,from}_bytes roundtrip
     nlp_bytes = nlp.to_bytes()
     nlp3 = English()
-    nlp3.add_pipe("trainable_lemmatizer")
+    nlp3.add_pipe("trainable_lemmatizer", config={"top_k": top_k})
     nlp3.from_bytes(nlp_bytes)
     doc3 = nlp3(test_text)
     assert doc3[0].lemma_ == "she"
     assert doc3[1].lemma_ == "like"
     assert doc3[2].lemma_ == "blue"
     assert doc3[3].lemma_ == "egg"
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_entity_linker.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_entity_linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from typing import Callable, Iterable, Dict, Any, cast
 
 import pytest
 from numpy.testing import assert_equal
 from thinc.types import Ragged
 
-from spacy import registry, util
+from spacy import registry, util, Language
 from spacy.attrs import ENT_KB_ID
 from spacy.compat import pickle
-from spacy.kb import Candidate, InMemoryLookupKB, get_candidates, KnowledgeBase
+from spacy.kb import Candidate, InMemoryLookupKB, KnowledgeBase
 from spacy.lang.en import English
 from spacy.ml import load_kb
-from spacy.ml.models.entity_linker import build_span_maker
+from spacy.ml.models.entity_linker import build_span_maker, get_candidates
 from spacy.pipeline import EntityLinker, TrainablePipe
-from spacy.pipeline.legacy import EntityLinker_v1
 from spacy.pipeline.tok2vec import DEFAULT_TOK2VEC_MODEL
 from spacy.scorer import Scorer
 from spacy.tests.util import make_tempdir
 from spacy.tokens import Span, Doc
 from spacy.training import Example
 from spacy.util import ensure_path
 from spacy.vocab import Vocab
@@ -105,26 +104,31 @@
     sent0 = sentences[0]
     ent = doc.ents[0]
     assert ent.start < sent0.end < ent.end
     assert sentences.index(ent.sent) == 0
 
 
 @pytest.mark.issue(7065)
-def test_issue7065_b():
+@pytest.mark.parametrize("entity_in_first_sentence", [True, False])
+def test_sentence_crossing_ents(entity_in_first_sentence: bool):
+    """Tests if NEL crashes if entities cross sentence boundaries and the first associated sentence doesn't have an
+    entity.
+    entity_in_prior_sentence (bool): Whether to include an entity in the first sentence associated with the
+    sentence-crossing entity.
+    """
     # Test that the NEL doesn't crash when an entity crosses a sentence boundary
     nlp = English()
     vector_length = 3
-    nlp.add_pipe("sentencizer")
     text = "Mahler 's Symphony No. 8 was beautiful."
-    entities = [(0, 6, "PERSON"), (10, 24, "WORK")]
-    links = {
-        (0, 6): {"Q7304": 1.0, "Q270853": 0.0},
-        (10, 24): {"Q7304": 0.0, "Q270853": 1.0},
-    }
-    sent_starts = [1, -1, 0, 0, 0, 0, 0, 0, 0]
+    entities = [(10, 24, "WORK")]
+    links = {(10, 24): {"Q7304": 0.0, "Q270853": 1.0}}
+    if entity_in_first_sentence:
+        entities.append((0, 6, "PERSON"))
+        links[(0, 6)] = {"Q7304": 1.0, "Q270853": 0.0}
+    sent_starts = [1, -1, 0, 0, 0, 1, 0, 0, 0]
     doc = nlp(text)
     example = Example.from_dict(
         doc, {"entities": entities, "links": links, "sent_starts": sent_starts}
     )
     train_examples = [example]
 
     def create_kb(vocab):
@@ -142,39 +146,22 @@
             entities=["Q7304"],
             probabilities=[1.0],
         )
         return mykb
 
     # Create the Entity Linker component and add it to the pipeline
     entity_linker = nlp.add_pipe("entity_linker", last=True)
-    entity_linker.set_kb(create_kb)
+    entity_linker.set_kb(create_kb)  # type: ignore
     # train the NEL pipe
     optimizer = nlp.initialize(get_examples=lambda: train_examples)
     for i in range(2):
-        losses = {}
-        nlp.update(train_examples, sgd=optimizer, losses=losses)
+        nlp.update(train_examples, sgd=optimizer)
 
-    # Add a custom rule-based component to mimick NER
-    patterns = [
-        {"label": "PERSON", "pattern": [{"LOWER": "mahler"}]},
-        {
-            "label": "WORK",
-            "pattern": [
-                {"LOWER": "symphony"},
-                {"LOWER": "no"},
-                {"LOWER": "."},
-                {"LOWER": "8"},
-            ],
-        },
-    ]
-    ruler = nlp.add_pipe("entity_ruler", before="entity_linker")
-    ruler.add_patterns(patterns)
-    # test the trained model - this should not throw E148
-    doc = nlp(text)
-    assert doc
+    # This shouldn't crash.
+    entity_linker.predict([example.reference])  # type: ignore
 
 
 def test_no_entities():
     # Test that having no entities doesn't crash the model
     TRAIN_DATA = [
         (
             "The sky is blue.",
@@ -350,14 +337,17 @@
         mykb.add_entity(entity="Q2", freq=5, entity_vector=[2])
 
 
 def test_kb_default(nlp):
     """Test that the default (empty) KB is loaded upon construction"""
     entity_linker = nlp.add_pipe("entity_linker", config={})
     assert len(entity_linker.kb) == 0
+    with pytest.raises(ValueError, match="E139"):
+        # this raises an error because the KB is empty
+        entity_linker.validate_kb()
     assert entity_linker.kb.get_size_entities() == 0
     assert entity_linker.kb.get_size_aliases() == 0
     # 64 is the default value from pipeline.entity_linker
     assert entity_linker.kb.entity_vector_length == 64
 
 
 def test_kb_custom_length(nlp):
@@ -459,24 +449,25 @@
     mykb.add_entity(entity="Q3", freq=5, entity_vector=[3])
 
     # adding aliases
     mykb.add_alias(alias="douglas", entities=["Q2", "Q3"], probabilities=[0.8, 0.1])
     mykb.add_alias(alias="adam", entities=["Q2"], probabilities=[0.9])
 
     # test the size of the relevant candidates
+    adam_ent_cands = get_candidates(mykb, adam_ent)
     assert len(get_candidates(mykb, douglas_ent)) == 2
-    assert len(get_candidates(mykb, adam_ent)) == 1
+    assert len(adam_ent_cands) == 1
     assert len(get_candidates(mykb, Adam_ent)) == 0  # default case sensitive
     assert len(get_candidates(mykb, shrubbery_ent)) == 0
 
     # test the content of the candidates
-    assert get_candidates(mykb, adam_ent)[0].entity_ == "Q2"
-    assert get_candidates(mykb, adam_ent)[0].alias_ == "adam"
-    assert_almost_equal(get_candidates(mykb, adam_ent)[0].entity_freq, 12)
-    assert_almost_equal(get_candidates(mykb, adam_ent)[0].prior_prob, 0.9)
+    assert adam_ent_cands[0].entity_id_ == "Q2"
+    assert adam_ent_cands[0].alias == "adam"
+    assert_almost_equal(adam_ent_cands[0].entity_freq, 12)
+    assert_almost_equal(adam_ent_cands[0].prior_prob, 0.9)
 
 
 def test_el_pipe_configuration(nlp):
     """Test correct candidate generation as part of the EL pipe"""
     nlp.add_pipe("sentencizer")
     pattern = {"label": "PERSON", "pattern": [{"LOWER": "douglas"}]}
     ruler = nlp.add_pipe("entity_ruler")
@@ -496,29 +487,29 @@
     text = "Douglas and douglas are not the same."
     doc = nlp(text)
     assert doc[0].ent_kb_id_ == "NIL"
     assert doc[1].ent_kb_id_ == ""
     assert doc[2].ent_kb_id_ == "Q2"
 
     def get_lowercased_candidates(kb, span):
-        return kb.get_alias_candidates(span.text.lower())
+        return kb._get_alias_candidates(span.text.lower())
 
     def get_lowercased_candidates_batch(kb, spans):
         return [get_lowercased_candidates(kb, span) for span in spans]
 
     @registry.misc("spacy.LowercaseCandidateGenerator.v1")
-    def create_candidates() -> Callable[
-        [InMemoryLookupKB, "Span"], Iterable[Candidate]
-    ]:
+    def create_candidates() -> (
+        Callable[[InMemoryLookupKB, "Span"], Iterable[Candidate]]
+    ):
         return get_lowercased_candidates
 
     @registry.misc("spacy.LowercaseCandidateBatchGenerator.v1")
-    def create_candidates_batch() -> Callable[
-        [InMemoryLookupKB, Iterable["Span"]], Iterable[Iterable[Candidate]]
-    ]:
+    def create_candidates_batch() -> (
+        Callable[[InMemoryLookupKB, Iterable["Span"]], Iterable[Iterable[Candidate]]]
+    ):
         return get_lowercased_candidates_batch
 
     # replace the pipe with a new one with with a different candidate generator
     entity_linker = nlp.replace_pipe(
         "entity_linker",
         "entity_linker",
         config={
@@ -555,32 +546,30 @@
     q2_hash = mykb.add_entity(entity="Q2", freq=12, entity_vector=[2])
     mykb.add_entity(entity="Q3", freq=5, entity_vector=[3])
 
     # adding aliases
     mykb.add_alias(alias="douglas", entities=["Q2", "Q3"], probabilities=[0.4, 0.1])
     adam_hash = mykb.add_alias(alias="adam", entities=["Q2"], probabilities=[0.9])
 
-    candidates = mykb.get_alias_candidates("adam")
+    candidates = mykb._get_alias_candidates("adam")
     assert len(candidates) == 1
-    assert candidates[0].entity == q2_hash
-    assert candidates[0].entity_ == "Q2"
-    assert candidates[0].alias == adam_hash
-    assert candidates[0].alias_ == "adam"
+    assert candidates[0].entity_id == q2_hash
+    assert candidates[0].entity_id_ == "Q2"
+    assert candidates[0].alias == "adam"
 
     with make_tempdir() as d:
         mykb.to_disk(d / "kb")
         kb_new_vocab = InMemoryLookupKB(Vocab(), entity_vector_length=1)
         kb_new_vocab.from_disk(d / "kb")
 
-        candidates = kb_new_vocab.get_alias_candidates("adam")
+        candidates = kb_new_vocab._get_alias_candidates("adam")
         assert len(candidates) == 1
-        assert candidates[0].entity == q2_hash
-        assert candidates[0].entity_ == "Q2"
-        assert candidates[0].alias == adam_hash
-        assert candidates[0].alias_ == "adam"
+        assert candidates[0].entity_id == q2_hash
+        assert candidates[0].entity_id_ == "Q2"
+        assert candidates[0].alias == "adam"
 
         assert kb_new_vocab.get_vector("Q2") == [2]
         assert_almost_equal(kb_new_vocab.get_prior_prob("Q2", "douglas"), 0.4)
 
 
 def test_append_alias(nlp):
     """Test that we can append additional alias-entity pairs"""
@@ -592,28 +581,28 @@
     mykb.add_entity(entity="Q3", freq=5, entity_vector=[3])
 
     # adding aliases
     mykb.add_alias(alias="douglas", entities=["Q2", "Q3"], probabilities=[0.4, 0.1])
     mykb.add_alias(alias="adam", entities=["Q2"], probabilities=[0.9])
 
     # test the size of the relevant candidates
-    assert len(mykb.get_alias_candidates("douglas")) == 2
+    assert len(mykb._get_alias_candidates("douglas")) == 2
 
     # append an alias
     mykb.append_alias(alias="douglas", entity="Q1", prior_prob=0.2)
 
     # test the size of the relevant candidates has been incremented
-    assert len(mykb.get_alias_candidates("douglas")) == 3
+    assert len(mykb._get_alias_candidates("douglas")) == 3
 
     # append the same alias-entity pair again should not work (will throw a warning)
     with pytest.warns(UserWarning):
         mykb.append_alias(alias="douglas", entity="Q1", prior_prob=0.3)
 
     # test the size of the relevant candidates remained unchanged
-    assert len(mykb.get_alias_candidates("douglas")) == 3
+    assert len(mykb._get_alias_candidates("douglas")) == 3
 
 
 @pytest.mark.filterwarnings("ignore:\\[W036")
 def test_append_invalid_alias(nlp):
     """Test that append an alias will throw an error if prior probs are exceeding 1"""
     mykb = InMemoryLookupKB(nlp.vocab, entity_vector_length=1)
 
@@ -902,19 +891,19 @@
     assert kb_1.entity_vector_length == kb_2.entity_vector_length
     assert kb_1.get_entity_strings() == kb_2.get_entity_strings()
     assert kb_1.get_vector("Q2146908") == kb_2.get_vector("Q2146908")
     assert kb_1.get_vector("Q66") == kb_2.get_vector("Q66")
     assert kb_2.contains_alias("Russ Cochran")
     assert kb_1.get_size_aliases() == kb_2.get_size_aliases()
     assert kb_1.get_alias_strings() == kb_2.get_alias_strings()
-    assert len(kb_1.get_alias_candidates("Russ Cochran")) == len(
-        kb_2.get_alias_candidates("Russ Cochran")
+    assert len(kb_1._get_alias_candidates("Russ Cochran")) == len(
+        kb_2._get_alias_candidates("Russ Cochran")
     )
-    assert len(kb_1.get_alias_candidates("Randomness")) == len(
-        kb_2.get_alias_candidates("Randomness")
+    assert len(kb_1._get_alias_candidates("Randomness")) == len(
+        kb_2._get_alias_candidates("Randomness")
     )
 
 
 def test_nel_to_bytes():
     # Test that a pipeline with an EL component can be converted to bytes
     def create_kb(vocab):
         kb = InMemoryLookupKB(vocab, entity_vector_length=3)
@@ -987,15 +976,14 @@
     assert scores["nel_micro_r"] == 2 / 4
 
 
 # fmt: off
 @pytest.mark.parametrize(
     "name,config",
     [
-        ("entity_linker", {"@architectures": "spacy.EntityLinker.v1", "tok2vec": DEFAULT_TOK2VEC_MODEL}),
         ("entity_linker", {"@architectures": "spacy.EntityLinker.v2", "tok2vec": DEFAULT_TOK2VEC_MODEL}),
     ],
 )
 # fmt: on
 def test_legacy_architectures(name, config):
     # Ensure that the legacy architectures still work
     vector_length = 3
@@ -1014,18 +1002,15 @@
             alias="Russ Cochran",
             entities=["Q2146908", "Q7381115"],
             probabilities=[0.5, 0.5],
         )
         return mykb
 
     entity_linker = nlp.add_pipe(name, config={"model": config})
-    if config["@architectures"] == "spacy.EntityLinker.v1":
-        assert isinstance(entity_linker, EntityLinker_v1)
-    else:
-        assert isinstance(entity_linker, EntityLinker)
+    assert isinstance(entity_linker, EntityLinker)
     entity_linker.set_kb(create_kb)
     optimizer = nlp.initialize(get_examples=lambda: train_examples)
 
     for i in range(2):
         losses = {}
         nlp.update(train_examples, sgd=optimizer, losses=losses)
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_entity_ruler.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_entity_ruler.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_functions.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_functions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_initialize.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_initialize.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_lemmatizer.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_models.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_models.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_morphologizer.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_morphologizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import cast
 import pytest
-from numpy.testing import assert_equal
+from numpy.testing import assert_equal, assert_almost_equal
+
+from thinc.api import get_current_ops
 
 from spacy import util
 from spacy.training import Example
 from spacy.lang.en import English
 from spacy.language import Language
 from spacy.tests.util import make_tempdir
 from spacy.morphology import Morphology
@@ -17,27 +19,53 @@
     nlp = Language()
     morphologizer = nlp.add_pipe("morphologizer")
     morphologizer.add_label("Feat=A")
     with pytest.raises(ValueError):
         morphologizer.add_label(9)
 
 
+TAGS = ["Feat=N", "Feat=V", "Feat=J"]
+
 TRAIN_DATA = [
     (
         "I like green eggs",
         {
             "morphs": ["Feat=N", "Feat=V", "Feat=J", "Feat=N"],
             "pos": ["NOUN", "VERB", "ADJ", "NOUN"],
         },
     ),
     # test combinations of morph+POS
     ("Eat blue ham", {"morphs": ["Feat=V", "", ""], "pos": ["", "ADJ", ""]}),
 ]
 
 
+def test_label_smoothing():
+    nlp = Language()
+    morph_no_ls = nlp.add_pipe("morphologizer", "no_label_smoothing")
+    morph_ls = nlp.add_pipe(
+        "morphologizer", "label_smoothing", config=dict(label_smoothing=0.05)
+    )
+    train_examples = []
+    losses = {}
+    for tag in TAGS:
+        morph_no_ls.add_label(tag)
+        morph_ls.add_label(tag)
+    for t in TRAIN_DATA:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    nlp.initialize(get_examples=lambda: train_examples)
+    tag_scores, bp_tag_scores = morph_ls.model.begin_update(
+        [eg.predicted for eg in train_examples]
+    )
+    ops = get_current_ops()
+    no_ls_grads = ops.to_numpy(morph_no_ls.get_loss(train_examples, tag_scores)[1][0])
+    ls_grads = ops.to_numpy(morph_ls.get_loss(train_examples, tag_scores)[1][0])
+    assert_almost_equal(ls_grads / no_ls_grads, 0.94285715)
+
+
 def test_no_label():
     nlp = Language()
     nlp.add_pipe("morphologizer")
     with pytest.raises(ValueError):
         nlp.initialize()
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_pipe_factories.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_pipe_factories.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_pipe_methods.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_pipe_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from thinc.api import get_current_ops
 
 import spacy
 from spacy.lang.en import English
 from spacy.lang.en.syntax_iterators import noun_chunks
 from spacy.language import Language
 from spacy.pipeline import TrainablePipe
+from spacy.strings import StringStore
 from spacy.tokens import Doc
 from spacy.training import Example
 from spacy.util import SimpleFrozenList, get_arg_names, make_tempdir
 from spacy.vocab import Vocab
 
 
 @pytest.fixture
@@ -127,15 +128,15 @@
 
 
 @pytest.mark.issue(5458)
 def test_issue5458():
     # Test that the noun chuncker does not generate overlapping spans
     # fmt: off
     words = ["In", "an", "era", "where", "markets", "have", "brought", "prosperity", "and", "empowerment", "."]
-    vocab = Vocab(strings=words)
+    vocab = Vocab(strings=StringStore(words))
     deps = ["ROOT", "det", "pobj", "advmod", "nsubj", "aux", "relcl", "dobj", "cc", "conj", "punct"]
     pos = ["ADP", "DET", "NOUN", "ADV", "NOUN", "AUX", "VERB", "NOUN", "CCONJ", "NOUN", "PUNCT"]
     heads = [0, 2, 0, 9, 6, 6, 2, 6, 7, 7, 0]
     # fmt: on
     en_doc = Doc(vocab, words=words, pos=pos, heads=heads, deps=deps)
     en_doc.noun_chunks_iterator = noun_chunks
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_sentencizer.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_sentencizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_senter.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_senter.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_span_ruler.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_span_ruler.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,26 +43,26 @@
 @pytest.fixture
 def person_org_date_patterns(person_org_patterns):
     return person_org_patterns + [{"label": "DATE", "pattern": "June 14th"}]
 
 
 def test_span_ruler_add_empty(patterns):
     """Test that patterns don't get added excessively."""
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler", config={"validate": True})
     ruler.add_patterns(patterns)
     pattern_count = sum(len(mm) for mm in ruler.matcher._patterns.values())
     assert pattern_count > 0
     ruler.add_patterns([])
     after_count = sum(len(mm) for mm in ruler.matcher._patterns.values())
     assert after_count == pattern_count
 
 
 def test_span_ruler_init(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(patterns)
     assert len(ruler) == len(patterns)
     assert len(ruler.labels) == 4
     assert "HELLO" in ruler
     assert "BYE" in ruler
     doc = nlp("hello world bye bye")
@@ -70,27 +70,27 @@
     assert doc.spans["ruler"][0].label_ == "HELLO"
     assert doc.spans["ruler"][0].id_ == "hello1"
     assert doc.spans["ruler"][1].label_ == "BYE"
     assert doc.spans["ruler"][1].id_ == ""
 
 
 def test_span_ruler_no_patterns_warns():
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     assert len(ruler) == 0
     assert len(ruler.labels) == 0
     assert nlp.pipe_names == ["span_ruler"]
     with pytest.warns(UserWarning):
         doc = nlp("hello world bye bye")
     assert len(doc.spans["ruler"]) == 0
 
 
 def test_span_ruler_init_patterns(patterns):
     # initialize with patterns
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     assert len(ruler.labels) == 0
     ruler.initialize(lambda: [], patterns=patterns)
     assert len(ruler.labels) == 4
     doc = nlp("hello world bye bye")
     assert doc.spans["ruler"][0].label_ == "HELLO"
     assert doc.spans["ruler"][1].label_ == "BYE"
@@ -106,86 +106,86 @@
     doc = nlp("hello world bye bye")
     assert doc.spans["ruler"][0].label_ == "HELLO"
     assert doc.spans["ruler"][1].label_ == "BYE"
 
 
 def test_span_ruler_init_clear(patterns):
     """Test that initialization clears patterns."""
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(patterns)
     assert len(ruler.labels) == 4
     ruler.initialize(lambda: [])
     assert len(ruler.labels) == 0
 
 
 def test_span_ruler_clear(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(patterns)
     assert len(ruler.labels) == 4
     doc = nlp("hello world")
     assert len(doc.spans["ruler"]) == 1
     ruler.clear()
     assert len(ruler.labels) == 0
     with pytest.warns(UserWarning):
         doc = nlp("hello world")
     assert len(doc.spans["ruler"]) == 0
 
 
 def test_span_ruler_existing(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler", config={"overwrite": False})
     ruler.add_patterns(patterns)
     doc = nlp.make_doc("OH HELLO WORLD bye bye")
     doc.spans["ruler"] = [doc[0:2]]
     doc = nlp(doc)
     assert len(doc.spans["ruler"]) == 3
     assert doc.spans["ruler"][0] == doc[0:2]
     assert doc.spans["ruler"][1].label_ == "HELLO"
     assert doc.spans["ruler"][1].id_ == "hello2"
     assert doc.spans["ruler"][2].label_ == "BYE"
     assert doc.spans["ruler"][2].id_ == ""
 
 
 def test_span_ruler_existing_overwrite(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler", config={"overwrite": True})
     ruler.add_patterns(patterns)
     doc = nlp.make_doc("OH HELLO WORLD bye bye")
     doc.spans["ruler"] = [doc[0:2]]
     doc = nlp(doc)
     assert len(doc.spans["ruler"]) == 2
     assert doc.spans["ruler"][0].label_ == "HELLO"
     assert doc.spans["ruler"][0].text == "HELLO"
     assert doc.spans["ruler"][1].label_ == "BYE"
 
 
 def test_span_ruler_serialize_bytes(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(patterns)
     assert len(ruler) == len(patterns)
     assert len(ruler.labels) == 4
     ruler_bytes = ruler.to_bytes()
-    new_nlp = spacy.blank("xx")
+    new_nlp = spacy.blank("mul")
     new_ruler = new_nlp.add_pipe("span_ruler")
     assert len(new_ruler) == 0
     assert len(new_ruler.labels) == 0
     new_ruler = new_ruler.from_bytes(ruler_bytes)
     assert len(new_ruler) == len(patterns)
     assert len(new_ruler.labels) == 4
     assert len(new_ruler.patterns) == len(ruler.patterns)
     for pattern in ruler.patterns:
         assert pattern in new_ruler.patterns
     assert sorted(new_ruler.labels) == sorted(ruler.labels)
 
 
 def test_span_ruler_validate():
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     validated_ruler = nlp.add_pipe(
         "span_ruler", name="validated_span_ruler", config={"validate": True}
     )
 
     valid_pattern = {"label": "HELLO", "pattern": [{"LOWER": "HELLO"}]}
     invalid_pattern = {"label": "HELLO", "pattern": [{"ASDF": "HELLO"}]}
@@ -199,32 +199,32 @@
 
     # invalid pattern raises error with validate
     with pytest.raises(MatchPatternError):
         validated_ruler.add_patterns([invalid_pattern])
 
 
 def test_span_ruler_properties(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler", config={"overwrite": True})
     ruler.add_patterns(patterns)
     assert sorted(ruler.labels) == sorted(set([p["label"] for p in patterns]))
 
 
 def test_span_ruler_overlapping_spans(overlapping_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(overlapping_patterns)
     doc = ruler(nlp.make_doc("foo bar baz"))
     assert len(doc.spans["ruler"]) == 2
     assert doc.spans["ruler"][0].label_ == "FOOBAR"
     assert doc.spans["ruler"][1].label_ == "BARBAZ"
 
 
 def test_span_ruler_scorer(overlapping_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(overlapping_patterns)
     text = "foo bar baz"
     pred_doc = ruler(nlp.make_doc(text))
     assert len(pred_doc.spans["ruler"]) == 2
     assert pred_doc.spans["ruler"][0].label_ == "FOOBAR"
     assert pred_doc.spans["ruler"][1].label_ == "BARBAZ"
@@ -239,62 +239,62 @@
 @pytest.mark.parametrize("n_process", [1, 2])
 def test_span_ruler_multiprocessing(n_process):
     if isinstance(get_current_ops, NumpyOps) or n_process < 2:
         texts = ["I enjoy eating Pizza Hut pizza."]
 
         patterns = [{"label": "FASTFOOD", "pattern": "Pizza Hut"}]
 
-        nlp = spacy.blank("xx")
+        nlp = spacy.blank("mul")
         ruler = nlp.add_pipe("span_ruler")
         ruler.add_patterns(patterns)
 
         for doc in nlp.pipe(texts, n_process=2):
             for ent in doc.spans["ruler"]:
                 assert ent.label_ == "FASTFOOD"
 
 
 def test_span_ruler_serialize_dir(patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(patterns)
     with make_tempdir() as d:
         ruler.to_disk(d / "test_ruler")
         ruler.from_disk(d / "test_ruler")  # read from an existing directory
         with pytest.raises(ValueError):
             ruler.from_disk(d / "non_existing_dir")  # read from a bad directory
 
 
 def test_span_ruler_remove_basic(person_org_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(person_org_patterns)
     doc = ruler(nlp.make_doc("Dina went to school"))
     assert len(ruler.patterns) == 3
     assert len(doc.spans["ruler"]) == 1
     assert doc.spans["ruler"][0].label_ == "PERSON"
     assert doc.spans["ruler"][0].text == "Dina"
     ruler.remove("PERSON")
     doc = ruler(nlp.make_doc("Dina went to school"))
     assert len(doc.spans["ruler"]) == 0
     assert len(ruler.patterns) == 2
 
 
 def test_span_ruler_remove_nonexisting_pattern(person_org_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(person_org_patterns)
     assert len(ruler.patterns) == 3
     with pytest.raises(ValueError):
         ruler.remove("NE")
     with pytest.raises(ValueError):
         ruler.remove_by_id("NE")
 
 
 def test_span_ruler_remove_several_patterns(person_org_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(person_org_patterns)
     doc = ruler(nlp.make_doc("Dina founded the company ACME."))
     assert len(ruler.patterns) == 3
     assert len(doc.spans["ruler"]) == 2
     assert doc.spans["ruler"][0].label_ == "PERSON"
     assert doc.spans["ruler"][0].text == "Dina"
@@ -310,15 +310,15 @@
     with pytest.warns(UserWarning):
         doc = ruler(nlp.make_doc("Dina founded the company ACME"))
         assert len(ruler.patterns) == 0
         assert len(doc.spans["ruler"]) == 0
 
 
 def test_span_ruler_remove_patterns_in_a_row(person_org_date_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(person_org_date_patterns)
     doc = ruler(nlp.make_doc("Dina founded the company ACME on June 14th"))
     assert len(doc.spans["ruler"]) == 3
     assert doc.spans["ruler"][0].label_ == "PERSON"
     assert doc.spans["ruler"][0].text == "Dina"
     assert doc.spans["ruler"][1].label_ == "ORG"
@@ -328,15 +328,15 @@
     ruler.remove("ORG")
     ruler.remove("DATE")
     doc = ruler(nlp.make_doc("Dina went to school"))
     assert len(doc.spans["ruler"]) == 1
 
 
 def test_span_ruler_remove_all_patterns(person_org_date_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     ruler.add_patterns(person_org_date_patterns)
     assert len(ruler.patterns) == 4
     ruler.remove("PERSON")
     assert len(ruler.patterns) == 3
     ruler.remove("ORG")
     assert len(ruler.patterns) == 1
@@ -344,15 +344,15 @@
     assert len(ruler.patterns) == 0
     with pytest.warns(UserWarning):
         doc = ruler(nlp.make_doc("Dina founded the company ACME on June 14th"))
         assert len(doc.spans["ruler"]) == 0
 
 
 def test_span_ruler_remove_and_add():
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler")
     patterns1 = [{"label": "DATE1", "pattern": "last time"}]
     ruler.add_patterns(patterns1)
     doc = ruler(
         nlp.make_doc("I saw him last time we met, this time he brought some flowers")
     )
     assert len(ruler.patterns) == 1
@@ -400,36 +400,36 @@
         )
     )
     assert len(ruler.patterns) == 2
     assert len(doc.spans["ruler"]) == 2
 
 
 def test_span_ruler_spans_filter(overlapping_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe(
         "span_ruler",
         config={"spans_filter": {"@misc": "spacy.first_longest_spans_filter.v1"}},
     )
     ruler.add_patterns(overlapping_patterns)
     doc = ruler(nlp.make_doc("foo bar baz"))
     assert len(doc.spans["ruler"]) == 1
     assert doc.spans["ruler"][0].label_ == "FOOBAR"
 
 
 def test_span_ruler_ents_default_filter(overlapping_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe("span_ruler", config={"annotate_ents": True})
     ruler.add_patterns(overlapping_patterns)
     doc = ruler(nlp.make_doc("foo bar baz"))
     assert len(doc.ents) == 1
     assert doc.ents[0].label_ == "FOOBAR"
 
 
 def test_span_ruler_ents_overwrite_filter(overlapping_patterns):
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe(
         "span_ruler",
         config={
             "annotate_ents": True,
             "overwrite": False,
             "ents_filter": {"@misc": "spacy.prioritize_new_ents_filter.v1"},
         },
@@ -448,15 +448,15 @@
     @registry.misc("test_pass_through_filter")
     def make_pass_through_filter():
         def pass_through_filter(spans1, spans2):
             return spans1 + spans2
 
         return pass_through_filter
 
-    nlp = spacy.blank("xx")
+    nlp = spacy.blank("mul")
     ruler = nlp.add_pipe(
         "span_ruler",
         config={
             "annotate_ents": True,
             "ents_filter": {"@misc": "test_pass_through_filter"},
         },
     )
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_spancat.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_spancat.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import pytest
 import numpy
 from numpy.testing import assert_array_equal, assert_almost_equal
-from thinc.api import get_current_ops, Ragged, fix_random_seed
+from thinc.api import get_current_ops, NumpyOps, Ragged, fix_random_seed
 
 from spacy import util
 from spacy.lang.en import English
 from spacy.language import Language
 from spacy.tokens import SpanGroup
 from spacy.tokens.span_groups import SpanGroups
 from spacy.training import Example
 from spacy.util import registry, make_tempdir
 
 OPS = get_current_ops()
 
 SPAN_KEY = "labeled_spans"
 
+SPANCAT_COMPONENTS = ["spancat", "spancat_singlelabel"]
+
 TRAIN_DATA = [
     ("Who is Shaka Khan?", {"spans": {SPAN_KEY: [(7, 17, "PERSON")]}}),
     (
         "I like London and Berlin.",
         {"spans": {SPAN_KEY: [(7, 13, "LOC"), (18, 24, "LOC")]}},
     ),
 ]
@@ -37,46 +39,50 @@
     train_examples = []
     for t in data:
         eg = Example.from_dict(nlp.make_doc(t[0]), t[1])
         train_examples.append(eg)
     return train_examples
 
 
-def test_no_label():
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+def test_no_label(name):
     nlp = Language()
-    nlp.add_pipe("spancat", config={"spans_key": SPAN_KEY})
+    nlp.add_pipe(name, config={"spans_key": SPAN_KEY})
     with pytest.raises(ValueError):
         nlp.initialize()
 
 
-def test_no_resize():
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+def test_no_resize(name):
     nlp = Language()
-    spancat = nlp.add_pipe("spancat", config={"spans_key": SPAN_KEY})
+    spancat = nlp.add_pipe(name, config={"spans_key": SPAN_KEY})
     spancat.add_label("Thing")
     spancat.add_label("Phrase")
     assert spancat.labels == ("Thing", "Phrase")
     nlp.initialize()
-    assert spancat.model.get_dim("nO") == 2
+    assert spancat.model.get_dim("nO") == spancat._n_labels
     # this throws an error because the spancat can't be resized after initialization
     with pytest.raises(ValueError):
         spancat.add_label("Stuff")
 
 
-def test_implicit_labels():
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+def test_implicit_labels(name):
     nlp = Language()
-    spancat = nlp.add_pipe("spancat", config={"spans_key": SPAN_KEY})
+    spancat = nlp.add_pipe(name, config={"spans_key": SPAN_KEY})
     assert len(spancat.labels) == 0
     train_examples = make_examples(nlp)
     nlp.initialize(get_examples=lambda: train_examples)
     assert spancat.labels == ("PERSON", "LOC")
 
 
-def test_explicit_labels():
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+def test_explicit_labels(name):
     nlp = Language()
-    spancat = nlp.add_pipe("spancat", config={"spans_key": SPAN_KEY})
+    spancat = nlp.add_pipe(name, config={"spans_key": SPAN_KEY})
     assert len(spancat.labels) == 0
     spancat.add_label("PERSON")
     spancat.add_label("LOC")
     nlp.initialize()
     assert spancat.labels == ("PERSON", "LOC")
 
 
@@ -98,36 +104,38 @@
     for text, spangroups in zip(texts, all_spans):
         assert isinstance(spangroups, SpanGroups)
         for key, spangroup in spangroups.items():
             assert isinstance(spangroup, SpanGroup)
             # XXX This fails with length 0 sometimes
             assert len(spangroup) > 0
             with pytest.raises(RuntimeError):
-                span = spangroup[0]
+                spangroup[0]
 
 
 @pytest.mark.parametrize(
     "max_positive,nr_results", [(None, 4), (1, 2), (2, 3), (3, 4), (4, 4)]
 )
-def test_make_spangroup(max_positive, nr_results):
+def test_make_spangroup_multilabel(max_positive, nr_results):
     fix_random_seed(0)
     nlp = Language()
     spancat = nlp.add_pipe(
         "spancat",
         config={"spans_key": SPAN_KEY, "threshold": 0.5, "max_positive": max_positive},
     )
     doc = nlp.make_doc("Greater London")
     ngram_suggester = registry.misc.get("spacy.ngram_suggester.v1")(sizes=[1, 2])
     indices = ngram_suggester([doc])[0].dataXd
     assert_array_equal(OPS.to_numpy(indices), numpy.asarray([[0, 1], [1, 2], [0, 2]]))
     labels = ["Thing", "City", "Person", "GreatCity"]
+    for label in labels:
+        spancat.add_label(label)
     scores = numpy.asarray(
         [[0.2, 0.4, 0.3, 0.1], [0.1, 0.6, 0.2, 0.4], [0.8, 0.7, 0.3, 0.9]], dtype="f"
     )
-    spangroup = spancat._make_span_group(doc, indices, scores, labels)
+    spangroup = spancat._make_span_group_multilabel(doc, indices, scores)
     assert len(spangroup) == nr_results
 
     # first span is always the second token "London"
     assert spangroup[0].text == "London"
     assert spangroup[0].label_ == "City"
     assert_almost_equal(0.6, spangroup.attrs["scores"][0], 5)
 
@@ -150,14 +158,138 @@
             assert_almost_equal(0.7, spangroup.attrs["scores"][2], 5)
 
     assert spangroup[-1].text == "Greater London"
     assert spangroup[-1].label_ == "GreatCity"
     assert_almost_equal(0.9, spangroup.attrs["scores"][-1], 5)
 
 
+@pytest.mark.parametrize(
+    "threshold,allow_overlap,nr_results",
+    [(0.05, True, 3), (0.05, False, 1), (0.5, True, 2), (0.5, False, 1)],
+)
+def test_make_spangroup_singlelabel(threshold, allow_overlap, nr_results):
+    fix_random_seed(0)
+    nlp = Language()
+    spancat = nlp.add_pipe(
+        "spancat",
+        config={
+            "spans_key": SPAN_KEY,
+            "threshold": threshold,
+            "max_positive": 1,
+        },
+    )
+    doc = nlp.make_doc("Greater London")
+    ngram_suggester = registry.misc.get("spacy.ngram_suggester.v1")(sizes=[1, 2])
+    indices = ngram_suggester([doc])[0].dataXd
+    assert_array_equal(OPS.to_numpy(indices), numpy.asarray([[0, 1], [1, 2], [0, 2]]))
+    labels = ["Thing", "City", "Person", "GreatCity"]
+    for label in labels:
+        spancat.add_label(label)
+    scores = numpy.asarray(
+        [[0.2, 0.4, 0.3, 0.1], [0.1, 0.6, 0.2, 0.4], [0.8, 0.7, 0.3, 0.9]], dtype="f"
+    )
+    spangroup = spancat._make_span_group_singlelabel(
+        doc, indices, scores, allow_overlap
+    )
+    if threshold > 0.4:
+        if allow_overlap:
+            assert spangroup[0].text == "London"
+            assert spangroup[0].label_ == "City"
+            assert_almost_equal(0.6, spangroup.attrs["scores"][0], 5)
+            assert spangroup[1].text == "Greater London"
+            assert spangroup[1].label_ == "GreatCity"
+            assert spangroup.attrs["scores"][1] == 0.9
+            assert_almost_equal(0.9, spangroup.attrs["scores"][1], 5)
+        else:
+            assert spangroup[0].text == "Greater London"
+            assert spangroup[0].label_ == "GreatCity"
+            assert spangroup.attrs["scores"][0] == 0.9
+    else:
+        if allow_overlap:
+            assert spangroup[0].text == "Greater"
+            assert spangroup[0].label_ == "City"
+            assert spangroup[1].text == "London"
+            assert spangroup[1].label_ == "City"
+            assert spangroup[2].text == "Greater London"
+            assert spangroup[2].label_ == "GreatCity"
+        else:
+            assert spangroup[0].text == "Greater London"
+
+
+def test_make_spangroup_negative_label():
+    fix_random_seed(0)
+    nlp_single = Language()
+    nlp_multi = Language()
+    spancat_single = nlp_single.add_pipe(
+        "spancat",
+        config={
+            "spans_key": SPAN_KEY,
+            "threshold": 0.1,
+            "max_positive": 1,
+        },
+    )
+    spancat_multi = nlp_multi.add_pipe(
+        "spancat",
+        config={
+            "spans_key": SPAN_KEY,
+            "threshold": 0.1,
+            "max_positive": 2,
+        },
+    )
+    spancat_single.add_negative_label = True
+    spancat_multi.add_negative_label = True
+    doc = nlp_single.make_doc("Greater London")
+    labels = ["Thing", "City", "Person", "GreatCity"]
+    for label in labels:
+        spancat_multi.add_label(label)
+        spancat_single.add_label(label)
+    ngram_suggester = registry.misc.get("spacy.ngram_suggester.v1")(sizes=[1, 2])
+    indices = ngram_suggester([doc])[0].dataXd
+    assert_array_equal(OPS.to_numpy(indices), numpy.asarray([[0, 1], [1, 2], [0, 2]]))
+    scores = numpy.asarray(
+        [
+            [0.2, 0.4, 0.3, 0.1, 0.1],
+            [0.1, 0.6, 0.2, 0.4, 0.9],
+            [0.8, 0.7, 0.3, 0.9, 0.1],
+        ],
+        dtype="f",
+    )
+    spangroup_multi = spancat_multi._make_span_group_multilabel(doc, indices, scores)
+    spangroup_single = spancat_single._make_span_group_singlelabel(doc, indices, scores)
+    assert len(spangroup_single) == 2
+    assert spangroup_single[0].text == "Greater"
+    assert spangroup_single[0].label_ == "City"
+    assert_almost_equal(0.4, spangroup_single.attrs["scores"][0], 5)
+    assert spangroup_single[1].text == "Greater London"
+    assert spangroup_single[1].label_ == "GreatCity"
+    assert spangroup_single.attrs["scores"][1] == 0.9
+    assert_almost_equal(0.9, spangroup_single.attrs["scores"][1], 5)
+
+    assert len(spangroup_multi) == 6
+    assert spangroup_multi[0].text == "Greater"
+    assert spangroup_multi[0].label_ == "City"
+    assert_almost_equal(0.4, spangroup_multi.attrs["scores"][0], 5)
+    assert spangroup_multi[1].text == "Greater"
+    assert spangroup_multi[1].label_ == "Person"
+    assert_almost_equal(0.3, spangroup_multi.attrs["scores"][1], 5)
+    assert spangroup_multi[2].text == "London"
+    assert spangroup_multi[2].label_ == "City"
+    assert_almost_equal(0.6, spangroup_multi.attrs["scores"][2], 5)
+    assert spangroup_multi[3].text == "London"
+    assert spangroup_multi[3].label_ == "GreatCity"
+    assert_almost_equal(0.4, spangroup_multi.attrs["scores"][3], 5)
+    assert spangroup_multi[4].text == "Greater London"
+    assert spangroup_multi[4].label_ == "Thing"
+    assert spangroup_multi[4].text == "Greater London"
+    assert_almost_equal(0.8, spangroup_multi.attrs["scores"][4], 5)
+    assert spangroup_multi[5].text == "Greater London"
+    assert spangroup_multi[5].label_ == "GreatCity"
+    assert_almost_equal(0.9, spangroup_multi.attrs["scores"][5], 5)
+
+
 def test_ngram_suggester(en_tokenizer):
     # test different n-gram lengths
     for size in [1, 2, 3]:
         ngram_suggester = registry.misc.get("spacy.ngram_suggester.v1")(sizes=[size])
         docs = [
             en_tokenizer(text)
             for text in [
@@ -270,14 +402,29 @@
     # one more variation
     suggester_factory = registry.misc.get("spacy.ngram_range_suggester.v1")
     range_suggester = suggester_factory(min_size=2, max_size=4)
     ngrams_3 = range_suggester(docs)
     assert_array_equal(OPS.to_numpy(ngrams_3.lengths), [0, 1, 3, 6, 9])
 
 
+def test_preset_spans_suggester():
+    nlp = Language()
+    docs = [nlp("This is an example."), nlp("This is the second example.")]
+    docs[0].spans[SPAN_KEY] = [docs[0][3:4]]
+    docs[1].spans[SPAN_KEY] = [docs[1][0:4], docs[1][3:5]]
+    suggester = registry.misc.get("spacy.preset_spans_suggester.v1")(spans_key=SPAN_KEY)
+    candidates = suggester(docs)
+    assert type(candidates) == Ragged
+    assert len(candidates) == 2
+    assert list(candidates.dataXd[0]) == [3, 4]
+    assert list(candidates.dataXd[1]) == [0, 4]
+    assert list(candidates.dataXd[2]) == [3, 5]
+    assert list(candidates.lengths) == [1, 2]
+
+
 def test_overfitting_IO():
     # Simple test to try and quickly overfit the spancat component - ensuring the ML models work correctly
     fix_random_seed(0)
     nlp = English()
     spancat = nlp.add_pipe("spancat", config={"spans_key": SPAN_KEY})
     train_examples = make_examples(nlp)
     optimizer = nlp.initialize(get_examples=lambda: train_examples)
@@ -292,27 +439,27 @@
     # test the trained model
     test_text = "I like London and Berlin"
     doc = nlp(test_text)
     assert doc.spans[spancat.key] == doc.spans[SPAN_KEY]
     spans = doc.spans[SPAN_KEY]
     assert len(spans) == 2
     assert len(spans.attrs["scores"]) == 2
-    assert min(spans.attrs["scores"]) > 0.9
+    assert min(spans.attrs["scores"]) > 0.8
     assert set([span.text for span in spans]) == {"London", "Berlin"}
     assert set([span.label_ for span in spans]) == {"LOC"}
 
     # Also test the results are still the same after IO
     with make_tempdir() as tmp_dir:
         nlp.to_disk(tmp_dir)
         nlp2 = util.load_model_from_path(tmp_dir)
         doc2 = nlp2(test_text)
         spans2 = doc2.spans[SPAN_KEY]
         assert len(spans2) == 2
         assert len(spans2.attrs["scores"]) == 2
-        assert min(spans2.attrs["scores"]) > 0.9
+        assert min(spans2.attrs["scores"]) > 0.8
         assert set([span.text for span in spans2]) == {"London", "Berlin"}
         assert set([span.label_ for span in spans2]) == {"LOC"}
 
     # Test scoring
     scores = nlp.evaluate(train_examples)
     assert f"spans_{SPAN_KEY}_f" in scores
     assert scores[f"spans_{SPAN_KEY}_p"] == 1.0
@@ -367,17 +514,17 @@
             "London",
             "Berlin",
             "London and Berlin",
         }
         assert set([span.label_ for span in spans2]) == {"LOC", "DOUBLE_LOC"}
 
 
-def test_zero_suggestions():
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+def test_zero_suggestions(name):
     # Test with a suggester that can return 0 suggestions
-
     @registry.misc("test_mixed_zero_suggester")
     def make_mixed_zero_suggester():
         def mixed_zero_suggester(docs, *, ops=None):
             if ops is None:
                 ops = get_current_ops()
             spans = []
             lengths = []
@@ -396,23 +543,23 @@
             return output
 
         return mixed_zero_suggester
 
     fix_random_seed(0)
     nlp = English()
     spancat = nlp.add_pipe(
-        "spancat",
+        name,
         config={
             "suggester": {"@misc": "test_mixed_zero_suggester"},
             "spans_key": SPAN_KEY,
         },
     )
     train_examples = make_examples(nlp)
     optimizer = nlp.initialize(get_examples=lambda: train_examples)
-    assert spancat.model.get_dim("nO") == 2
+    assert spancat.model.get_dim("nO") == spancat._n_labels
     assert set(spancat.labels) == {"LOC", "PERSON"}
 
     nlp.update(train_examples, sgd=optimizer)
     # empty doc
     nlp("")
     # single doc with zero suggestions
     nlp("one")
@@ -420,17 +567,18 @@
     nlp("two two")
     # batch with mixed zero/one suggestions
     list(nlp.pipe(["one", "two two", "three three three", "", "four four four four"]))
     # batch with no suggestions
     list(nlp.pipe(["", "one", "three three three"]))
 
 
-def test_set_candidates():
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+def test_set_candidates(name):
     nlp = Language()
-    spancat = nlp.add_pipe("spancat", config={"spans_key": SPAN_KEY})
+    spancat = nlp.add_pipe(name, config={"spans_key": SPAN_KEY})
     train_examples = make_examples(nlp)
     nlp.initialize(get_examples=lambda: train_examples)
     texts = [
         "Just a sentence.",
         "I like London and Berlin",
         "I like Berlin",
         "I eat ham.",
@@ -460,7 +608,25 @@
     assert "spancat" not in doc.activations
 
     spancat.save_activations = True
     doc = nlp("This is a test.")
     assert set(doc.activations["spancat"].keys()) == {"indices", "scores"}
     assert doc.activations["spancat"]["indices"].shape == (12, 2)
     assert doc.activations["spancat"]["scores"].shape == (12, nO)
+
+
+@pytest.mark.parametrize("name", SPANCAT_COMPONENTS)
+@pytest.mark.parametrize("n_process", [1, 2])
+def test_spancat_multiprocessing(name, n_process):
+    if isinstance(get_current_ops, NumpyOps) or n_process < 2:
+        nlp = Language()
+        spancat = nlp.add_pipe(name, config={"spans_key": SPAN_KEY})
+        train_examples = make_examples(nlp)
+        nlp.initialize(get_examples=lambda: train_examples)
+        texts = [
+            "Just a sentence.",
+            "I like London and Berlin",
+            "I like Berlin",
+            "I eat ham.",
+        ]
+        docs = list(nlp.pipe(texts, n_process=n_process))
+        assert len(docs) == len(texts)
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_tagger.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_tagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import cast
 import pytest
-from numpy.testing import assert_equal
+from numpy.testing import assert_equal, assert_almost_equal
 from spacy.attrs import TAG
 
 from spacy import util
 from spacy.training import Example
 from spacy.lang.en import English
 from spacy.language import Language
 from spacy.pipeline import TrainablePipe
-from thinc.api import compounding
+from thinc.api import compounding, get_current_ops
 
 from ..util import make_tempdir
 
 
 @pytest.mark.issue(4348)
 def test_issue4348():
     """Test that training the tagger with empty data, doesn't throw errors"""
@@ -67,14 +67,38 @@
             "words": ["He", "hate", "s", "green", "eggs"],
             "tags": ["", "V", "S", "J", ""],
         },
     ),
 ]
 
 
+def test_label_smoothing():
+    nlp = Language()
+    tagger_no_ls = nlp.add_pipe("tagger", "no_label_smoothing")
+    tagger_ls = nlp.add_pipe(
+        "tagger", "label_smoothing", config=dict(label_smoothing=0.05)
+    )
+    train_examples = []
+    losses = {}
+    for tag in TAGS:
+        tagger_no_ls.add_label(tag)
+        tagger_ls.add_label(tag)
+    for t in TRAIN_DATA:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    nlp.initialize(get_examples=lambda: train_examples)
+    tag_scores, bp_tag_scores = tagger_ls.model.begin_update(
+        [eg.predicted for eg in train_examples]
+    )
+    ops = get_current_ops()
+    no_ls_grads = ops.to_numpy(tagger_no_ls.get_loss(train_examples, tag_scores)[1][0])
+    ls_grads = ops.to_numpy(tagger_ls.get_loss(train_examples, tag_scores)[1][0])
+    assert_almost_equal(ls_grads / no_ls_grads, 0.925)
+
+
 def test_no_label():
     nlp = Language()
     nlp.add_pipe("tagger")
     with pytest.raises(ValueError):
         nlp.initialize()
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_textcat.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/pipeline/test_tok2vec.py` & `spacy-4.0.0.dev1/spacy/tests/pipeline/test_tok2vec.py`

 * *Files 10% similar despite different names*

```diff
@@ -536,7 +536,90 @@
     assert cats0["preference"] < 0.1
     assert cats0["imperative"] > 0.9
     cats1 = docs[1].cats
     assert cats1["preference"] > 0.1
     assert cats1["imperative"] < 0.9
     assert [t.tag_ for t in docs[0]] == ["V", "J", "N"]
     assert [t.tag_ for t in docs[1]] == ["N", "V", "J", "N"]
+
+
+cfg_string_distillation = """
+    [nlp]
+    lang = "en"
+    pipeline = ["tok2vec","tagger"]
+
+    [components]
+
+    [components.tagger]
+    factory = "tagger"
+
+    [components.tagger.model]
+    @architectures = "spacy.Tagger.v2"
+    nO = null
+
+    [components.tagger.model.tok2vec]
+    @architectures = "spacy.Tok2VecListener.v1"
+    width = ${components.tok2vec.model.encode.width}
+
+    [components.tok2vec]
+    factory = "tok2vec"
+
+    [components.tok2vec.model]
+    @architectures = "spacy.Tok2Vec.v2"
+
+    [components.tok2vec.model.embed]
+    @architectures = "spacy.MultiHashEmbed.v2"
+    width = ${components.tok2vec.model.encode.width}
+    rows = [2000, 1000, 1000, 1000]
+    attrs = ["NORM", "PREFIX", "SUFFIX", "SHAPE"]
+    include_static_vectors = false
+
+    [components.tok2vec.model.encode]
+    @architectures = "spacy.MaxoutWindowEncoder.v2"
+    width = 96
+    depth = 4
+    window_size = 1
+    maxout_pieces = 3
+    """
+
+
+def test_tok2vec_distillation_teacher_annotations():
+    orig_config = Config().from_str(cfg_string_distillation)
+    teacher_nlp = util.load_model_from_config(
+        orig_config, auto_fill=True, validate=True
+    )
+    student_nlp = util.load_model_from_config(
+        orig_config, auto_fill=True, validate=True
+    )
+
+    train_examples_teacher = []
+    train_examples_student = []
+    for t in TRAIN_DATA:
+        train_examples_teacher.append(
+            Example.from_dict(teacher_nlp.make_doc(t[0]), t[1])
+        )
+        train_examples_student.append(
+            Example.from_dict(student_nlp.make_doc(t[0]), t[1])
+        )
+
+    optimizer = teacher_nlp.initialize(lambda: train_examples_teacher)
+    student_nlp.initialize(lambda: train_examples_student)
+
+    # Since Language.distill creates a copy of the examples to use as
+    # its internal teacher/student docs, we'll need to monkey-patch the
+    # tok2vec pipe's distill method.
+    student_tok2vec = student_nlp.get_pipe("tok2vec")
+    student_tok2vec._old_distill = student_tok2vec.distill
+
+    def tok2vec_distill_wrapper(
+        self,
+        teacher_pipe,
+        examples,
+        **kwargs,
+    ):
+        assert all(not eg.reference.tensor.any() for eg in examples)
+        out = self._old_distill(teacher_pipe, examples, **kwargs)
+        assert all(eg.reference.tensor.any() for eg in examples)
+        return out
+
+    student_tok2vec.distill = tok2vec_distill_wrapper.__get__(student_tok2vec, Tok2Vec)
+    student_nlp.distill(teacher_nlp, train_examples_student, sgd=optimizer, losses={})
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_resource_warning.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_resource_warning.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 
 def entity_linker():
     nlp = Language()
 
     def create_kb(vocab):
         kb = InMemoryLookupKB(vocab, entity_vector_length=1)
-        kb.add_entity("test", 0.0, zeros((1, 1), dtype="f"))
+        kb.add_entity("test", 0.0, zeros((1,), dtype="f"))
         return kb
 
     entity_linker = nlp.add_pipe("entity_linker")
     entity_linker.set_kb(create_kb)
     # need to add model for two reasons:
     # 1. no model leads to error in serialization,
     # 2. the affected line is the one for model serialization
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_config.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from catalogue import RegistryError
 from thinc.api import Config, ConfigValidationError
 
 import spacy
 from spacy.lang.de import German
 from spacy.lang.en import English
 from spacy.language import DEFAULT_CONFIG, DEFAULT_CONFIG_PRETRAIN_PATH
+from spacy.language import DEFAULT_CONFIG_DISTILL_PATH
 from spacy.language import Language
 from spacy.ml.models import MaxoutWindowEncoder, MultiHashEmbed
 from spacy.ml.models import build_tb_parser_model, build_Tok2Vec_model
-from spacy.schemas import ConfigSchema, ConfigSchemaPretrain
+from spacy.schemas import ConfigSchema, ConfigSchemaDistill, ConfigSchemaPretrain
 from spacy.util import load_config, load_config_from_str
 from spacy.util import load_model_from_config, registry
 
 from ..util import make_tempdir
 
 nlp_config_string = """
 [paths]
@@ -62,14 +63,68 @@
 @architectures = "spacy.Tagger.v2"
 
 [components.tagger.model.tok2vec]
 @architectures = "spacy.Tok2VecListener.v1"
 width = ${components.tok2vec.model.width}
 """
 
+distill_config_string = """
+[paths]
+train = null
+dev = null
+
+[corpora]
+
+[corpora.train]
+@readers = "spacy.Corpus.v1"
+path = ${paths.train}
+
+[corpora.dev]
+@readers = "spacy.Corpus.v1"
+path = ${paths.dev}
+
+[training]
+
+[training.batcher]
+@batchers = "spacy.batch_by_words.v1"
+size = 666
+
+[nlp]
+lang = "en"
+pipeline = ["tok2vec", "tagger"]
+
+[components]
+
+[components.tok2vec]
+factory = "tok2vec"
+
+[components.tok2vec.model]
+@architectures = "spacy.HashEmbedCNN.v1"
+pretrained_vectors = null
+width = 342
+depth = 4
+window_size = 1
+embed_size = 2000
+maxout_pieces = 3
+subword_features = true
+
+[components.tagger]
+factory = "tagger"
+
+[components.tagger.model]
+@architectures = "spacy.Tagger.v2"
+
+[components.tagger.model.tok2vec]
+@architectures = "spacy.Tok2VecListener.v1"
+width = ${components.tok2vec.model.width}
+
+[distill]
+"""
+
+
 pretrain_config_string = """
 [paths]
 train = null
 dev = null
 
 [corpora]
 
@@ -197,14 +252,22 @@
         bad_cfg = {"yolo": {}}
         load_model_from_config(Config(bad_cfg), auto_fill=True)
     with pytest.raises(ValueError):
         bad_cfg = {"pipeline": {"foo": "bar"}}
         load_model_from_config(Config(bad_cfg), auto_fill=True)
 
 
+def test_nlp_from_distillation_config():
+    """Test that the default distillation config validates properly"""
+    config = Config().from_str(distill_config_string)
+    distill_config = load_config(DEFAULT_CONFIG_DISTILL_PATH)
+    filled = config.merge(distill_config)
+    registry.resolve(filled["distillation"], schema=ConfigSchemaDistill)
+
+
 def test_create_nlp_from_pretraining_config():
     """Test that the default pretraining config validates properly"""
     config = Config().from_str(pretrain_config_string)
     pretrain_config = load_config(DEFAULT_CONFIG_PRETRAIN_PATH)
     filled = config.merge(pretrain_config)
     registry.resolve(filled["pretraining"], schema=ConfigSchemaPretrain)
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_doc.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_doc.py`

 * *Files 8% similar despite different names*

```diff
@@ -209,10 +209,17 @@
     assert not new_doc.user_data
     new_doc = Doc(en_vocab).from_bytes(doc.to_bytes(exclude=["user_data"]))
     assert not new_doc.user_data
 
 
 def test_serialize_doc_span_groups(en_vocab):
     doc = Doc(en_vocab, words=["hello", "world", "!"])
-    doc.spans["content"] = [doc[0:2]]
+    span = doc[0:2]
+    span.label_ = "test_serialize_doc_span_groups_label"
+    span.id_ = "test_serialize_doc_span_groups_id"
+    span.kb_id_ = "test_serialize_doc_span_groups_kb_id"
+    doc.spans["content"] = [span]
     new_doc = Doc(en_vocab).from_bytes(doc.to_bytes())
     assert len(new_doc.spans["content"]) == 1
+    assert new_doc.spans["content"][0].label_ == "test_serialize_doc_span_groups_label"
+    assert new_doc.spans["content"][0].id_ == "test_serialize_doc_span_groups_id"
+    assert new_doc.spans["content"][0].kb_id_ == "test_serialize_doc_span_groups_kb_id"
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_docbin.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_docbin.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,28 +45,35 @@
         attrs=["LEMMA", "ENT_IOB", "ENT_TYPE", "NORM", "ENT_ID"], store_user_data=True
     )
     texts = ["Some text", "Lots of texts...", "..."]
     cats = {"A": 0.5}
     nlp = English()
     for doc in nlp.pipe(texts):
         doc.cats = cats
-        doc.spans["start"] = [doc[0:2]]
+        span = doc[0:2]
+        span.label_ = "UNUSUAL_SPAN_LABEL"
+        span.id_ = "UNUSUAL_SPAN_ID"
+        span.kb_id_ = "UNUSUAL_SPAN_KB_ID"
+        doc.spans["start"] = [span]
         doc[0].norm_ = "UNUSUAL_TOKEN_NORM"
         doc[0].ent_id_ = "UNUSUAL_TOKEN_ENT_ID"
         doc_bin.add(doc)
     bytes_data = doc_bin.to_bytes()
 
     # Deserialize later, e.g. in a new process
     nlp = spacy.blank("en")
     doc_bin = DocBin().from_bytes(bytes_data)
     reloaded_docs = list(doc_bin.get_docs(nlp.vocab))
     for i, doc in enumerate(reloaded_docs):
         assert doc.text == texts[i]
         assert doc.cats == cats
         assert len(doc.spans) == 1
+        assert doc.spans["start"][0].label_ == "UNUSUAL_SPAN_LABEL"
+        assert doc.spans["start"][0].id_ == "UNUSUAL_SPAN_ID"
+        assert doc.spans["start"][0].kb_id_ == "UNUSUAL_SPAN_KB_ID"
         assert doc[0].norm_ == "UNUSUAL_TOKEN_NORM"
         assert doc[0].ent_id_ == "UNUSUAL_TOKEN_ENT_ID"
 
 
 def test_serialize_doc_bin_unknown_spaces(en_vocab):
     doc1 = Doc(en_vocab, words=["that", "'s"])
     assert doc1.has_unknown_spaces
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_extension_attrs.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_extension_attrs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_kb.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_kb.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from typing import Callable
+from pathlib import Path
+from typing import Callable, Iterable, Any, Dict
 
-from spacy import util
-from spacy.util import ensure_path, registry, load_model_from_config
+import srsly
+
+from spacy import util, Errors
+from spacy.util import ensure_path, registry, load_model_from_config, SimpleFrozenList
 from spacy.kb.kb_in_memory import InMemoryLookupKB
 from spacy.vocab import Vocab
 from thinc.api import Config
 
 from ..util import make_tempdir
 from numpy import zeros
 
@@ -59,27 +62,29 @@
     assert kb.get_size_aliases() == 3
     for alias_string in ["double07", "guy", "random"]:
         assert alias_string in kb.get_alias_strings()
     for alias_string in ["nothingness", "", "randomnoise"]:
         assert alias_string not in kb.get_alias_strings()
 
     # check candidates & probabilities
-    candidates = sorted(kb.get_alias_candidates("double07"), key=lambda x: x.entity_)
+    candidates = sorted(
+        kb._get_alias_candidates("double07"), key=lambda x: x.entity_id_
+    )
     assert len(candidates) == 2
 
-    assert candidates[0].entity_ == "Q007"
+    assert candidates[0].entity_id_ == "Q007"
     assert 6.999 < candidates[0].entity_freq < 7.01
     assert candidates[0].entity_vector == [0, 0, 7]
-    assert candidates[0].alias_ == "double07"
+    assert candidates[0].alias == "double07"
     assert 0.899 < candidates[0].prior_prob < 0.901
 
-    assert candidates[1].entity_ == "Q17"
+    assert candidates[1].entity_id_ == "Q17"
     assert 1.99 < candidates[1].entity_freq < 2.01
     assert candidates[1].entity_vector == [7, 1, 0]
-    assert candidates[1].alias_ == "double07"
+    assert candidates[1].alias == "double07"
     assert 0.099 < candidates[1].prior_prob < 0.101
 
 
 def test_serialize_subclassed_kb():
     """Check that IO of a custom KB works fine as part of an EL pipe."""
 
     config_string = """
@@ -87,36 +92,86 @@
     lang = "en"
     pipeline = ["entity_linker"]
 
     [components]
 
     [components.entity_linker]
     factory = "entity_linker"
-
+    
+    [components.entity_linker.generate_empty_kb]
+    @misc = "kb_test.CustomEmptyKB.v1"
+    
     [initialize]
 
     [initialize.components]
 
     [initialize.components.entity_linker]
 
     [initialize.components.entity_linker.kb_loader]
-    @misc = "spacy.CustomKB.v1"
+    @misc = "kb_test.CustomKB.v1"
     entity_vector_length = 342
     custom_field = 666
     """
 
     class SubInMemoryLookupKB(InMemoryLookupKB):
         def __init__(self, vocab, entity_vector_length, custom_field):
             super().__init__(vocab, entity_vector_length)
             self.custom_field = custom_field
 
-    @registry.misc("spacy.CustomKB.v1")
+        def to_disk(self, path, exclude: Iterable[str] = SimpleFrozenList()):
+            """We overwrite InMemoryLookupKB.to_disk() to ensure that self.custom_field is stored as well."""
+            path = ensure_path(path)
+            if not path.exists():
+                path.mkdir(parents=True)
+            if not path.is_dir():
+                raise ValueError(Errors.E928.format(loc=path))
+
+            def serialize_custom_fields(file_path: Path) -> None:
+                srsly.write_json(file_path, {"custom_field": self.custom_field})
+
+            serialize = {
+                "contents": lambda p: self.write_contents(p),
+                "strings.json": lambda p: self.vocab.strings.to_disk(p),
+                "custom_fields": lambda p: serialize_custom_fields(p),
+            }
+            util.to_disk(path, serialize, exclude)
+
+        def from_disk(self, path, exclude: Iterable[str] = SimpleFrozenList()):
+            """We overwrite InMemoryLookupKB.from_disk() to ensure that self.custom_field is loaded as well."""
+            path = ensure_path(path)
+            if not path.exists():
+                raise ValueError(Errors.E929.format(loc=path))
+            if not path.is_dir():
+                raise ValueError(Errors.E928.format(loc=path))
+
+            def deserialize_custom_fields(file_path: Path) -> None:
+                self.custom_field = srsly.read_json(file_path)["custom_field"]
+
+            deserialize: Dict[str, Callable[[Any], Any]] = {
+                "contents": lambda p: self.read_contents(p),
+                "strings.json": lambda p: self.vocab.strings.from_disk(p),
+                "custom_fields": lambda p: deserialize_custom_fields(p),
+            }
+            util.from_disk(path, deserialize, exclude)
+
+    @registry.misc("kb_test.CustomEmptyKB.v1")
+    def empty_custom_kb() -> Callable[[Vocab, int], SubInMemoryLookupKB]:
+        def empty_kb_factory(vocab: Vocab, entity_vector_length: int):
+            return SubInMemoryLookupKB(
+                vocab=vocab,
+                entity_vector_length=entity_vector_length,
+                custom_field=0,
+            )
+
+        return empty_kb_factory
+
+    @registry.misc("kb_test.CustomKB.v1")
     def custom_kb(
         entity_vector_length: int, custom_field: int
-    ) -> Callable[[Vocab], InMemoryLookupKB]:
+    ) -> Callable[[Vocab], SubInMemoryLookupKB]:
         def custom_kb_factory(vocab):
             kb = SubInMemoryLookupKB(
                 vocab=vocab,
                 entity_vector_length=entity_vector_length,
                 custom_field=custom_field,
             )
             kb.add_entity("random_entity", 0.0, zeros(entity_vector_length))
@@ -135,10 +190,10 @@
 
     # Make sure the custom KB is serialized correctly
     with make_tempdir() as tmp_dir:
         nlp.to_disk(tmp_dir)
         nlp2 = util.load_model_from_path(tmp_dir)
         entity_linker2 = nlp2.get_pipe("entity_linker")
         # After IO, the KB is the standard one
-        assert type(entity_linker2.kb) == InMemoryLookupKB
+        assert type(entity_linker2.kb) == SubInMemoryLookupKB
         assert entity_linker2.kb.entity_vector_length == 342
-        assert not hasattr(entity_linker2.kb, "custom_field")
+        assert entity_linker2.kb.custom_field == 666
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_language.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_language.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_pipeline.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         ner2.from_disk(output_dir)
         assert len(ner2.labels) == 2
 
 
 @pytest.mark.issue(4725)
 def test_issue4725_1():
     """Ensure the pickling of the NER goes well"""
-    vocab = Vocab(vectors_name="test_vocab_add_vector")
+    vocab = Vocab()
     nlp = English(vocab=vocab)
     config = {
         "update_with_oracle_cut_size": 111,
     }
     ner = nlp.create_pipe("ner", config=config)
     with make_tempdir() as tmp_path:
         with (tmp_path / "ner.pkl").open("wb") as file_:
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_span_groups.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_span_groups.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/serialize/test_serialize_vocab_strings.py` & `spacy-4.0.0.dev1/spacy/tests/serialize/test_serialize_vocab_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 from spacy.tokens import Doc
 from spacy.util import ensure_path, load_model
 from spacy.vectors import Vectors
 from spacy.vocab import Vocab
 
 from ..util import make_tempdir
 
-test_strings = [([], []), (["rats", "are", "cute"], ["i", "like", "rats"])]
-test_strings_attrs = [(["rats", "are", "cute"], "Hello")]
+test_strings = [
+    (StringStore(), StringStore()),
+    (StringStore(["rats", "are", "cute"]), StringStore(["i", "like", "rats"])),
+]
+test_strings_attrs = [(StringStore(["rats", "are", "cute"]), "Hello")]
 
 
 @pytest.mark.issue(599)
 def test_issue599(en_vocab):
     doc = Doc(en_vocab)
     doc2 = Doc(doc.vocab)
     doc2.from_bytes(doc.to_bytes())
@@ -77,15 +80,15 @@
 
 @pytest.mark.parametrize("strings1,strings2", test_strings)
 def test_serialize_vocab_roundtrip_bytes(strings1, strings2):
     vocab1 = Vocab(strings=strings1)
     vocab2 = Vocab(strings=strings2)
     vocab1_b = vocab1.to_bytes()
     vocab2_b = vocab2.to_bytes()
-    if strings1 == strings2:
+    if strings1.to_bytes() == strings2.to_bytes():
         assert vocab1_b == vocab2_b
     else:
         assert vocab1_b != vocab2_b
     vocab1 = vocab1.from_bytes(vocab1_b)
     assert vocab1.to_bytes() == vocab1_b
     new_vocab1 = Vocab().from_bytes(vocab1_b)
     assert new_vocab1.to_bytes() == vocab1_b
@@ -113,41 +116,43 @@
             assert [s for s in vocab1_d.strings] != [s for s in vocab2_d.strings]
 
 
 @pytest.mark.parametrize("strings,lex_attr", test_strings_attrs)
 def test_serialize_vocab_lex_attrs_bytes(strings, lex_attr):
     vocab1 = Vocab(strings=strings)
     vocab2 = Vocab()
-    vocab1[strings[0]].norm_ = lex_attr
-    assert vocab1[strings[0]].norm_ == lex_attr
-    assert vocab2[strings[0]].norm_ != lex_attr
+    s = next(iter(vocab1.strings))
+    vocab1[s].norm_ = lex_attr
+    assert vocab1[s].norm_ == lex_attr
+    assert vocab2[s].norm_ != lex_attr
     vocab2 = vocab2.from_bytes(vocab1.to_bytes())
-    assert vocab2[strings[0]].norm_ == lex_attr
+    assert vocab2[s].norm_ == lex_attr
 
 
 @pytest.mark.parametrize("strings,lex_attr", test_strings_attrs)
 def test_deserialize_vocab_seen_entries(strings, lex_attr):
     # Reported in #2153
     vocab = Vocab(strings=strings)
     vocab.from_bytes(vocab.to_bytes())
     assert len(vocab.strings) == len(strings)
 
 
 @pytest.mark.parametrize("strings,lex_attr", test_strings_attrs)
 def test_serialize_vocab_lex_attrs_disk(strings, lex_attr):
     vocab1 = Vocab(strings=strings)
     vocab2 = Vocab()
-    vocab1[strings[0]].norm_ = lex_attr
-    assert vocab1[strings[0]].norm_ == lex_attr
-    assert vocab2[strings[0]].norm_ != lex_attr
+    s = next(iter(vocab1.strings))
+    vocab1[s].norm_ = lex_attr
+    assert vocab1[s].norm_ == lex_attr
+    assert vocab2[s].norm_ != lex_attr
     with make_tempdir() as d:
         file_path = d / "vocab"
         vocab1.to_disk(file_path)
         vocab2 = vocab2.from_disk(file_path)
-    assert vocab2[strings[0]].norm_ == lex_attr
+    assert vocab2[s].norm_ == lex_attr
 
 
 @pytest.mark.parametrize("strings1,strings2", test_strings)
 def test_serialize_stringstore_roundtrip_bytes(strings1, strings2):
     sstore1 = StringStore(strings=strings1)
     sstore2 = StringStore(strings=strings2)
     sstore1_b = sstore1.to_bytes()
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_cli.py` & `spacy-4.0.0.dev1/spacy/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import math
 from collections import Counter
 from typing import Tuple, List, Dict, Any
-import pkg_resources
 import time
 from pathlib import Path
 
 import spacy
 import numpy
 import pytest
 import srsly
 from click import NoSuchOption
 from packaging.specifiers import SpecifierSet
 from thinc.api import Config, ConfigValidationError
+from spacy.tokens import DocBin
 
 from spacy import about
 from spacy.cli import info
 from spacy.cli._util import is_subpath_of, load_project_config, walk_directory
 from spacy.cli._util import parse_config_overrides, string_to_list
 from spacy.cli._util import substitute_project_variables
 from spacy.cli._util import validate_project_commands
@@ -24,15 +24,17 @@
 from spacy.cli.debug_data import _compile_gold, _get_labels_from_model
 from spacy.cli.debug_data import _get_labels_from_spancat
 from spacy.cli.debug_data import _get_distribution, _get_kl_divergence
 from spacy.cli.debug_data import _get_span_characteristics
 from spacy.cli.debug_data import _print_span_characteristics
 from spacy.cli.debug_data import _get_spans_length_freq_dist
 from spacy.cli.download import get_compatibility, get_version
+from spacy.cli.evaluate import render_parses
 from spacy.cli.init_config import RECOMMENDATIONS, init_config, fill_config
+from spacy.cli.init_pipeline import _init_labels
 from spacy.cli.package import get_third_party_dependencies
 from spacy.cli.package import _is_permitted_package_name
 from spacy.cli.project.remote_storage import RemoteStorage
 from spacy.cli.project.run import _check_requirements
 from spacy.cli.validate import get_model_pkgs
 from spacy.cli.apply import apply
 from spacy.cli.find_threshold import find_threshold
@@ -43,15 +45,14 @@
 from spacy.tokens import Doc, DocBin
 from spacy.tokens.span import Span
 from spacy.training import Example, docs_to_json, offsets_to_biluo_tags
 from spacy.training.converters import conll_ner_to_docs, conllu_to_docs
 from spacy.training.converters import iob_to_docs
 from spacy.util import ENV_VARS, get_minor_version, load_model_from_config, load_config
 
-from ..cli.init_pipeline import _init_labels
 from .util import make_tempdir
 
 
 @pytest.mark.issue(4665)
 def test_cli_converters_conllu_empty_heads_ner():
     """
     conllu_to_docs should not raise an exception if the HEAD column contains an
@@ -141,14 +142,78 @@
         cfg = load_project_config(d)
         # Check that the directories are interpolated and created correctly
         assert os.path.exists(d / "cfg")
         assert os.path.exists(d / f"{lang_var}_model")
     assert cfg["commands"][0]["script"][0] == f"hello {lang_var}"
 
 
+@pytest.mark.issue(12566)
+@pytest.mark.parametrize(
+    "factory,output_file",
+    [("deps", "parses.html"), ("ents", "entities.html"), ("spans", "spans.html")],
+)
+def test_issue12566(factory: str, output_file: str):
+    """
+    Test if all displaCy types (ents, dep, spans) produce an HTML file
+    """
+    with make_tempdir() as tmp_dir:
+        # Create sample spaCy file
+        doc_json = {
+            "ents": [
+                {"end": 54, "label": "nam_adj_country", "start": 44},
+                {"end": 83, "label": "nam_liv_person", "start": 69},
+                {"end": 100, "label": "nam_pro_title_book", "start": 86},
+            ],
+            "spans": {
+                "sc": [
+                    {"end": 54, "kb_id": "", "label": "nam_adj_country", "start": 44},
+                    {"end": 83, "kb_id": "", "label": "nam_liv_person", "start": 69},
+                    {
+                        "end": 100,
+                        "kb_id": "",
+                        "label": "nam_pro_title_book",
+                        "start": 86,
+                    },
+                ]
+            },
+            "text": "Niedawno czytał em nową książkę znakomitego szkockiego medioznawcy , "
+            "Briana McNaira - Cultural Chaos .",
+            "tokens": [
+                # fmt: off
+                {"id": 0, "start": 0, "end": 8, "tag": "ADV", "pos": "ADV", "morph": "Degree=Pos", "lemma": "niedawno", "dep": "advmod", "head": 1, },
+                {"id": 1, "start": 9, "end": 15, "tag": "PRAET", "pos": "VERB", "morph": "Animacy=Hum|Aspect=Imp|Gender=Masc|Mood=Ind|Number=Sing|Tense=Past|VerbForm=Fin|Voice=Act", "lemma": "czytać", "dep": "ROOT", "head": 1, },
+                {"id": 2, "start": 16, "end": 18, "tag": "AGLT", "pos": "NOUN", "morph": "Animacy=Inan|Case=Ins|Gender=Masc|Number=Sing", "lemma": "em", "dep": "iobj", "head": 1, },
+                {"id": 3, "start": 19, "end": 23, "tag": "ADJ", "pos": "ADJ", "morph": "Case=Acc|Degree=Pos|Gender=Fem|Number=Sing", "lemma": "nowy", "dep": "amod", "head": 4, },
+                {"id": 4, "start": 24, "end": 31, "tag": "SUBST", "pos": "NOUN", "morph": "Case=Acc|Gender=Fem|Number=Sing", "lemma": "książka", "dep": "obj", "head": 1, },
+                {"id": 5, "start": 32, "end": 43, "tag": "ADJ", "pos": "ADJ", "morph": "Animacy=Nhum|Case=Gen|Degree=Pos|Gender=Masc|Number=Sing", "lemma": "znakomit", "dep": "acl", "head": 4, },
+                {"id": 6, "start": 44, "end": 54, "tag": "ADJ", "pos": "ADJ", "morph": "Animacy=Hum|Case=Gen|Degree=Pos|Gender=Masc|Number=Sing", "lemma": "szkockiy", "dep": "amod", "head": 7, },
+                {"id": 7, "start": 55, "end": 66, "tag": "SUBST", "pos": "NOUN", "morph": "Animacy=Hum|Case=Gen|Gender=Masc|Number=Sing", "lemma": "medioznawca", "dep": "iobj", "head": 5, },
+                {"id": 8, "start": 67, "end": 68, "tag": "INTERP", "pos": "PUNCT", "morph": "PunctType=Comm", "lemma": ",", "dep": "punct", "head": 9, },
+                {"id": 9, "start": 69, "end": 75, "tag": "SUBST", "pos": "PROPN", "morph": "Animacy=Hum|Case=Gen|Gender=Masc|Number=Sing", "lemma": "Brian", "dep": "nmod", "head": 4, },
+                {"id": 10, "start": 76, "end": 83, "tag": "SUBST", "pos": "PROPN", "morph": "Animacy=Hum|Case=Gen|Gender=Masc|Number=Sing", "lemma": "McNair", "dep": "flat", "head": 9, },
+                {"id": 11, "start": 84, "end": 85, "tag": "INTERP", "pos": "PUNCT", "morph": "PunctType=Dash", "lemma": "-", "dep": "punct", "head": 12, },
+                {"id": 12, "start": 86, "end": 94, "tag": "SUBST", "pos": "PROPN", "morph": "Animacy=Inan|Case=Nom|Gender=Masc|Number=Sing", "lemma": "Cultural", "dep": "conj", "head": 4, },
+                {"id": 13, "start": 95, "end": 100, "tag": "SUBST", "pos": "NOUN", "morph": "Animacy=Inan|Case=Nom|Gender=Masc|Number=Sing", "lemma": "Chaos", "dep": "flat", "head": 12, },
+                {"id": 14, "start": 101, "end": 102, "tag": "INTERP", "pos": "PUNCT", "morph": "PunctType=Peri", "lemma": ".", "dep": "punct", "head": 1, },
+                # fmt: on
+            ],
+        }
+
+        # Create a .spacy file
+        nlp = spacy.blank("pl")
+        doc = Doc(nlp.vocab).from_json(doc_json)
+
+        # Run the evaluate command and check if the html files exist
+        render_parses(
+            docs=[doc], output_path=tmp_dir, model_name="", limit=1, **{factory: True}
+        )
+
+        assert (tmp_dir / output_file).is_file()
+
+
 def test_cli_info():
     nlp = Dutch()
     nlp.add_pipe("textcat")
     with make_tempdir() as tmp_dir:
         nlp.to_disk(tmp_dir)
         raw_data = info(tmp_dir, exclude=[""])
         assert raw_data["lang"] == "nl"
@@ -549,15 +614,22 @@
     with pytest.raises(SystemExit):
         parse_config_overrides([])
     del os.environ[ENV_VARS.CONFIG_OVERRIDES]
 
 
 @pytest.mark.parametrize("lang", ["en", "nl"])
 @pytest.mark.parametrize(
-    "pipeline", [["tagger", "parser", "ner"], [], ["ner", "textcat", "sentencizer"]]
+    "pipeline",
+    [
+        ["tagger", "parser", "ner"],
+        [],
+        ["ner", "textcat", "sentencizer"],
+        ["morphologizer", "spancat", "entity_linker"],
+        ["spancat_singlelabel", "textcat_multilabel"],
+    ],
 )
 @pytest.mark.parametrize("optimize", ["efficiency", "accuracy"])
 @pytest.mark.parametrize("pretraining", [True, False])
 def test_init_config(lang, pipeline, optimize, pretraining):
     # TODO: add more tests and also check for GPU with transformers
     config = init_config(
         lang=lang,
@@ -614,26 +686,24 @@
     ],
 )
 def test_string_to_list_intify(value):
     assert string_to_list(value, intify=False) == ["1", "2", "3"]
     assert string_to_list(value, intify=True) == [1, 2, 3]
 
 
-@pytest.mark.skip(reason="Temporarily skip for dev version")
 def test_download_compatibility():
     spec = SpecifierSet("==" + about.__version__)
     spec.prereleases = False
     if about.__version__ in spec:
         model_name = "en_core_web_sm"
         compatibility = get_compatibility()
         version = get_version(model_name, compatibility)
         assert get_minor_version(about.__version__) == get_minor_version(version)
 
 
-@pytest.mark.skip(reason="Temporarily skip for dev version")
 def test_validate_compatibility_table():
     spec = SpecifierSet("==" + about.__version__)
     spec.prereleases = False
     if about.__version__ in spec:
         model_pkgs, compat = get_model_pkgs()
         spacy_version = get_minor_version(about.__version__)
         current_compat = compat.get(spacy_version, {})
@@ -1015,16 +1085,14 @@
         filename = "a.txt"
         remote = RemoteStorage(d / "root", str(d / "remote"))
         assert remote.pull(filename, command_hash="aaaa") is None
         assert remote.pull(filename) is None
 
 
 def test_cli_find_threshold(capsys):
-    thresholds = numpy.linspace(0, 1, 10)
-
     def make_examples(nlp: Language) -> List[Example]:
         docs: List[Example] = []
 
         for t in [
             (
                 "I am angry and confused in the Bank of America.",
                 {
@@ -1072,43 +1140,39 @@
         # mostly as a smoke test.
         nlp, examples = init_nlp()
         DocBin(docs=[example.reference for example in examples]).to_disk(
             docs_dir / "docs.spacy"
         )
         with make_tempdir() as nlp_dir:
             nlp.to_disk(nlp_dir)
-            res = find_threshold(
+            best_threshold, best_score, res = find_threshold(
                 model=nlp_dir,
                 data_path=docs_dir / "docs.spacy",
                 pipe_name="tc_multi",
                 threshold_key="threshold",
                 scores_key="cats_macro_f",
                 silent=True,
             )
-            assert res[0] != thresholds[0]
-            assert thresholds[0] < res[0] < thresholds[9]
-            assert res[1] == 1.0
-            assert res[2][1.0] == 0.0
+            assert best_score == max(res.values())
+            assert res[1.0] == 0.0
 
         # Test with spancat.
         nlp, _ = init_nlp((("spancat", {}),))
         with make_tempdir() as nlp_dir:
             nlp.to_disk(nlp_dir)
-            res = find_threshold(
+            best_threshold, best_score, res = find_threshold(
                 model=nlp_dir,
                 data_path=docs_dir / "docs.spacy",
                 pipe_name="spancat",
                 threshold_key="threshold",
                 scores_key="spans_sc_f",
                 silent=True,
             )
-            assert res[0] != thresholds[0]
-            assert thresholds[0] < res[0] < thresholds[8]
-            assert res[1] >= 0.6
-            assert res[2][1.0] == 0.0
+            assert best_score == max(res.values())
+            assert res[1.0] == 0.0
 
         # Having multiple textcat_multilabel components should work, since the name has to be specified.
         nlp, _ = init_nlp((("textcat_multilabel", {}),))
         with make_tempdir() as nlp_dir:
             nlp.to_disk(nlp_dir)
             assert find_threshold(
                 model=nlp_dir,
@@ -1130,14 +1194,15 @@
                     pipe_name="_",
                     threshold_key="threshold",
                     scores_key="cats_macro_f",
                     silent=True,
                 )
 
 
+@pytest.mark.filterwarnings("ignore::DeprecationWarning")
 @pytest.mark.parametrize(
     "reqs,output",
     [
         [
             """
             spacy
 
@@ -1162,14 +1227,16 @@
             """# comment
              spacyunknowndoesnotexist12345""",
             (True, False),
         ],
     ],
 )
 def test_project_check_requirements(reqs, output):
+    import pkg_resources
+
     # excessive guard against unlikely package name
     try:
         pkg_resources.require("spacyunknowndoesnotexist12345")
     except pkg_resources.DistributionNotFound:
         assert output == _check_requirements([req.strip() for req in reqs.split("\n")])
 
 
@@ -1205,7 +1272,73 @@
 
         assert (len(walk_directory(d))) == 7
         assert (len(walk_directory(d, suffix=None))) == 7
         assert (len(walk_directory(d, suffix="json"))) == 1
         assert (len(walk_directory(d, suffix="iob"))) == 2
         assert (len(walk_directory(d, suffix="conll"))) == 3
         assert (len(walk_directory(d, suffix="pdf"))) == 0
+
+
+def test_debug_data_trainable_lemmatizer_basic():
+    examples = [
+        ("She likes green eggs", {"lemmas": ["she", "like", "green", "egg"]}),
+        ("Eat blue ham", {"lemmas": ["eat", "blue", "ham"]}),
+    ]
+    nlp = Language()
+    train_examples = []
+    for t in examples:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    data = _compile_gold(train_examples, ["trainable_lemmatizer"], nlp, True)
+    # ref test_edit_tree_lemmatizer::test_initialize_from_labels
+    # this results in 4 trees
+    assert len(data["lemmatizer_trees"]) == 4
+
+
+def test_debug_data_trainable_lemmatizer_partial():
+    partial_examples = [
+        # partial annotation
+        ("She likes green eggs", {"lemmas": ["", "like", "green", ""]}),
+        # misaligned partial annotation
+        (
+            "He hates green eggs",
+            {
+                "words": ["He", "hat", "es", "green", "eggs"],
+                "lemmas": ["", "hat", "e", "green", ""],
+            },
+        ),
+    ]
+    nlp = Language()
+    train_examples = []
+    for t in partial_examples:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    data = _compile_gold(train_examples, ["trainable_lemmatizer"], nlp, True)
+    assert data["partial_lemma_annotations"] == 2
+
+
+def test_debug_data_trainable_lemmatizer_low_cardinality():
+    low_cardinality_examples = [
+        ("She likes green eggs", {"lemmas": ["no", "no", "no", "no"]}),
+        ("Eat blue ham", {"lemmas": ["no", "no", "no"]}),
+    ]
+    nlp = Language()
+    train_examples = []
+    for t in low_cardinality_examples:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    data = _compile_gold(train_examples, ["trainable_lemmatizer"], nlp, True)
+    assert data["n_low_cardinality_lemmas"] == 2
+
+
+def test_debug_data_trainable_lemmatizer_not_annotated():
+    unannotated_examples = [
+        ("She likes green eggs", {}),
+        ("Eat blue ham", {}),
+    ]
+    nlp = Language()
+    train_examples = []
+    for t in unannotated_examples:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    data = _compile_gold(train_examples, ["trainable_lemmatizer"], nlp, True)
+    assert data["no_lemma_annotations"] == 2
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_displacy.py` & `spacy-4.0.0.dev1/spacy/tests/test_displacy.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,14 +271,28 @@
         {"lemma": None, "text": words[3], "tag": pos[3]},
     ]
     assert deps["arcs"] == [
         {"start": 0, "end": 1, "label": "nsubj", "dir": "left"},
         {"start": 2, "end": 3, "label": "det", "dir": "left"},
         {"start": 1, "end": 3, "label": "attr", "dir": "right"},
     ]
+    # Test that displacy.parse_deps converts Span to Doc
+    deps = displacy.parse_deps(doc[:])
+    assert isinstance(deps, dict)
+    assert deps["words"] == [
+        {"lemma": None, "text": words[0], "tag": pos[0]},
+        {"lemma": None, "text": words[1], "tag": pos[1]},
+        {"lemma": None, "text": words[2], "tag": pos[2]},
+        {"lemma": None, "text": words[3], "tag": pos[3]},
+    ]
+    assert deps["arcs"] == [
+        {"start": 0, "end": 1, "label": "nsubj", "dir": "left"},
+        {"start": 2, "end": 3, "label": "det", "dir": "left"},
+        {"start": 1, "end": 3, "label": "attr", "dir": "right"},
+    ]
 
 
 def test_displacy_invalid_arcs():
     renderer = DependencyRenderer()
     words = [{"text": "This", "tag": "DET"}, {"text": "is", "tag": "VERB"}]
     arcs = [
         {"start": 0, "end": 1, "label": "nsubj", "dir": "left"},
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_language.py` & `spacy-4.0.0.dev1/spacy/tests/test_language.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,29 +6,81 @@
 from spacy.scorer import Scorer
 from spacy.tokens import Doc, Span
 from spacy.vocab import Vocab
 from spacy.training import Example
 from spacy.lang.en import English
 from spacy.lang.de import German
 from spacy.util import registry, ignore_error, raise_error, find_matching_language
+from spacy.util import load_model_from_config
 import spacy
-from thinc.api import CupyOps, NumpyOps, get_current_ops
+from thinc.api import Config, CupyOps, NumpyOps, get_array_module, get_current_ops
 
 from .util import add_vecs_to_vocab, assert_docs_equal
 
 
 try:
     import torch
 
     # Ensure that we don't deadlock in multiprocessing tests.
     torch.set_num_threads(1)
     torch.set_num_interop_threads(1)
 except ImportError:
     pass
 
+TAGGER_CFG_STRING = """
+    [nlp]
+    lang = "en"
+    pipeline = ["tok2vec","tagger"]
+
+    [components]
+
+    [components.tagger]
+    factory = "tagger"
+
+    [components.tagger.model]
+    @architectures = "spacy.Tagger.v2"
+    nO = null
+
+    [components.tagger.model.tok2vec]
+    @architectures = "spacy.Tok2VecListener.v1"
+    width = ${components.tok2vec.model.encode.width}
+
+    [components.tok2vec]
+    factory = "tok2vec"
+
+    [components.tok2vec.model]
+    @architectures = "spacy.Tok2Vec.v2"
+
+    [components.tok2vec.model.embed]
+    @architectures = "spacy.MultiHashEmbed.v1"
+    width = ${components.tok2vec.model.encode.width}
+    rows = [2000, 1000, 1000, 1000]
+    attrs = ["NORM", "PREFIX", "SUFFIX", "SHAPE"]
+    include_static_vectors = false
+
+    [components.tok2vec.model.encode]
+    @architectures = "spacy.MaxoutWindowEncoder.v2"
+    width = 96
+    depth = 4
+    window_size = 1
+    maxout_pieces = 3
+    """
+
+
+TAGGER_TRAIN_DATA = [
+    ("I like green eggs", {"tags": ["N", "V", "J", "N"]}),
+    ("Eat blue ham", {"tags": ["V", "J", "N"]}),
+]
+
+
+TAGGER_TRAIN_DATA = [
+    ("I like green eggs", {"tags": ["N", "V", "J", "N"]}),
+    ("Eat blue ham", {"tags": ["V", "J", "N"]}),
+]
+
 
 def evil_component(doc):
     if "2" in doc.text:
         raise ValueError("no dice")
     return doc
 
 
@@ -42,15 +94,15 @@
     if not doc.has_annotation("SENT_START"):
         raise ValueError("no sents")
     return doc
 
 
 def warn_error(proc_name, proc, docs, e):
     logger = logging.getLogger("spacy")
-    logger.warning(f"Trouble with component {proc_name}.")
+    logger.warning("Trouble with component %s.", proc_name)
 
 
 @pytest.fixture
 def nlp():
     nlp = Language(Vocab())
     textcat = nlp.add_pipe("textcat")
     for label in ("POSITIVE", "NEGATIVE"):
@@ -81,14 +133,52 @@
     # Create examples badly
     with pytest.raises(ValueError):
         example = Example.from_dict(doc, None)
     with pytest.raises(KeyError):
         example = Example.from_dict(doc, wrongkeyannots)
 
 
+def test_language_update_updates():
+    config = Config().from_str(TAGGER_CFG_STRING)
+    nlp = load_model_from_config(config, auto_fill=True, validate=True)
+
+    train_examples = []
+    for t in TAGGER_TRAIN_DATA:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    optimizer = nlp.initialize(get_examples=lambda: train_examples)
+
+    docs_before_update = list(nlp.pipe([eg.predicted.copy() for eg in train_examples]))
+    nlp.update(train_examples, sgd=optimizer)
+    docs_after_update = list(nlp.pipe([eg.predicted.copy() for eg in train_examples]))
+
+    xp = get_array_module(docs_after_update[0].tensor)
+    assert xp.any(
+        xp.not_equal(docs_before_update[0].tensor, docs_after_update[0].tensor)
+    )
+
+
+def test_language_update_does_not_update_with_sgd_false():
+    config = Config().from_str(TAGGER_CFG_STRING)
+    nlp = load_model_from_config(config, auto_fill=True, validate=True)
+
+    train_examples = []
+    for t in TAGGER_TRAIN_DATA:
+        train_examples.append(Example.from_dict(nlp.make_doc(t[0]), t[1]))
+
+    nlp.initialize(get_examples=lambda: train_examples)
+
+    docs_before_update = list(nlp.pipe([eg.predicted.copy() for eg in train_examples]))
+    nlp.update(train_examples, sgd=False)
+    docs_after_update = list(nlp.pipe([eg.predicted.copy() for eg in train_examples]))
+
+    xp = get_array_module(docs_after_update[0].tensor)
+    xp.testing.assert_equal(docs_before_update[0].tensor, docs_after_update[0].tensor)
+
+
 def test_language_evaluate(nlp):
     text = "hello world"
     annots = {"doc_annotation": {"cats": {"POSITIVE": 1.0, "NEGATIVE": 0.0}}}
     doc = Doc(nlp.vocab, words=text.split(" "))
     example = Example.from_dict(doc, annots)
     scores = nlp.evaluate([example])
     assert scores["speed"] > 0
@@ -654,19 +744,20 @@
 @pytest.mark.parametrize(
     "lang,target",
     [
         ("en", "en"),
         ("fra", "fr"),
         ("fre", "fr"),
         ("iw", "he"),
+        ("is", "isl"),
         ("mo", "ro"),
-        ("mul", "xx"),
+        ("mul", "mul"),
         ("no", "nb"),
         ("pt-BR", "pt"),
-        ("xx", "xx"),
+        ("xx", "mul"),
         ("zh-Hans", "zh"),
         ("zh-Hant", None),
         ("zxx", None),
     ],
 )
 def test_language_matching(lang, target):
     """
@@ -679,19 +770,19 @@
 @pytest.mark.parametrize(
     "lang,target",
     [
         ("en", "en"),
         ("fra", "fr"),
         ("fre", "fr"),
         ("iw", "he"),
+        ("is", "isl"),
         ("mo", "ro"),
-        ("mul", "xx"),
+        ("xx", "mul"),
         ("no", "nb"),
         ("pt-BR", "pt"),
-        ("xx", "xx"),
         ("zh-Hans", "zh"),
     ],
 )
 def test_blank_languages(lang, target):
     """
     Test that we can get spacy.blank in various languages, including codes
     that are defined to be equivalent or that match by CLDR language matching.
@@ -795,7 +886,70 @@
     @Language.component("test_component_bad_pipe")
     def bad_pipe(doc):
         return doc.text
 
     nlp.add_pipe("test_component_bad_pipe")
     with pytest.raises(ValueError, match="instead of a Doc"):
         nlp("text")
+
+
+@pytest.mark.slow
+@pytest.mark.parametrize("teacher_tagger_name", ["tagger", "teacher_tagger"])
+def test_distill(teacher_tagger_name):
+    teacher = English()
+    teacher_tagger = teacher.add_pipe("tagger", name=teacher_tagger_name)
+    train_examples = []
+    for t in TAGGER_TRAIN_DATA:
+        train_examples.append(Example.from_dict(teacher.make_doc(t[0]), t[1]))
+
+    optimizer = teacher.initialize(get_examples=lambda: train_examples)
+
+    for i in range(50):
+        losses = {}
+        teacher.update(train_examples, sgd=optimizer, losses=losses)
+    assert losses[teacher_tagger_name] < 0.00001
+
+    student = English()
+    student_tagger = student.add_pipe("tagger")
+    student_tagger.min_tree_freq = 1
+    student_tagger.initialize(
+        get_examples=lambda: train_examples, labels=teacher_tagger.label_data
+    )
+
+    distill_examples = [
+        Example.from_dict(teacher.make_doc(t[0]), {}) for t in TAGGER_TRAIN_DATA
+    ]
+
+    student_to_teacher = (
+        None
+        if teacher_tagger.name == student_tagger.name
+        else {student_tagger.name: teacher_tagger.name}
+    )
+
+    for i in range(50):
+        losses = {}
+        student.distill(
+            teacher,
+            distill_examples,
+            sgd=optimizer,
+            losses=losses,
+            student_to_teacher=student_to_teacher,
+        )
+    assert losses["tagger"] < 0.00001
+
+    test_text = "I like blue eggs"
+    doc = student(test_text)
+    assert doc[0].tag_ == "N"
+    assert doc[1].tag_ == "V"
+    assert doc[2].tag_ == "J"
+    assert doc[3].tag_ == "N"
+
+    # Do an extra update to check if annotates works, though we can't really
+    # validate the resuls, since the annotations are ephemeral.
+    student.distill(
+        teacher,
+        distill_examples,
+        sgd=optimizer,
+        losses=losses,
+        student_to_teacher=student_to_teacher,
+        annotates=["tagger"],
+    )
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_misc.py` & `spacy-4.0.0.dev1/spacy/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_models.py` & `spacy-4.0.0.dev1/spacy/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_pickles.py` & `spacy-4.0.0.dev1/spacy/tests/test_pickles.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_scorer.py` & `spacy-4.0.0.dev1/spacy/tests/test_scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,22 @@
     example.predicted[1].is_sent_start = False
     scores = scorer.score([example])
     assert scores["token_acc"] == 0.5
     assert scores["token_p"] == 0.5
     assert scores["token_r"] == approx(0.33333333)
     assert scores["token_f"] == 0.4
 
+    # per-component scoring
+    scorer = Scorer()
+    scores = scorer.score([example], per_component=True)
+    assert scores["tokenizer"]["token_acc"] == 0.5
+    assert scores["tokenizer"]["token_p"] == 0.5
+    assert scores["tokenizer"]["token_r"] == approx(0.33333333)
+    assert scores["tokenizer"]["token_f"] == 0.4
+
 
 def test_sents(sented_doc):
     scorer = Scorer()
     gold = {"sent_starts": [t.sent_start for t in sented_doc]}
     example = Example.from_dict(sented_doc, gold)
     scores = scorer.score([example])
     assert scores["sents_f"] == 1.0
@@ -274,14 +282,21 @@
     assert results["pos_acc"] == 0.9
     assert results["morph_acc"] == approx(0.8)
     assert results["morph_micro_f"] == approx(0.8461538)
     assert results["morph_per_feat"]["NounType"]["f"] == 1.0
     assert results["morph_per_feat"]["Poss"]["f"] == 0.0
     assert results["morph_per_feat"]["Number"]["f"] == approx(0.72727272)
 
+    # per-component scoring
+    scorer = Scorer()
+    results = scorer.score([example], per_component=True)
+    assert results["tagger"]["tag_acc"] == 0.9
+    assert results["morphologizer"]["pos_acc"] == 0.9
+    assert results["morphologizer"]["morph_acc"] == approx(0.8)
+
 
 def test_partial_annotation(en_tokenizer):
     pred_doc = en_tokenizer("a b c d e")
     pred_doc[0].tag_ = "A"
     pred_doc[0].pos_ = "X"
     pred_doc[0].set_morph("Feat=Val")
     pred_doc[0].dep_ = "dep"
@@ -419,22 +434,22 @@
     spans.append(gold.char_span(8, 12, label="ORG"))
     gold.spans[key] = spans
 
     def span_getter(doc, span_key):
         return doc.spans[span_key]
 
     # Predict exactly the same, but overlapping spans will be discarded
-    pred.spans[key] = spans
+    pred.spans[key] = gold.spans[key].copy(doc=pred)
     eg = Example(pred, gold)
     scores = Scorer.score_spans([eg], attr=key, getter=span_getter)
     assert scores[f"{key}_p"] == 1.0
     assert scores[f"{key}_r"] < 1.0
 
     # Allow overlapping, now both precision and recall should be 100%
-    pred.spans[key] = spans
+    pred.spans[key] = gold.spans[key].copy(doc=pred)
     eg = Example(pred, gold)
     scores = Scorer.score_spans([eg], attr=key, getter=span_getter, allow_overlap=True)
     assert scores[f"{key}_p"] == 1.0
     assert scores[f"{key}_r"] == 1.0
 
     # Change the predicted labels
     new_spans = [Span(pred, span.start, span.end, label="WRONG") for span in spans]
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_symbols.py` & `spacy-4.0.0.dev1/spacy/tests/test_symbols.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/test_ty.py` & `spacy-4.0.0.dev1/spacy/tests/test_ty.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/sun.txt` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/sun.txt`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/test_exceptions.py` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/test_explain.py` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/test_explain.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     pytest.param("ga", marks=pytest.mark.slow()),
     pytest.param("he", marks=pytest.mark.slow()),
     pytest.param("hi", marks=pytest.mark.slow()),
     pytest.param("hr", marks=pytest.mark.slow()),
     "hu",
     pytest.param("id", marks=pytest.mark.slow()),
     pytest.param("it", marks=pytest.mark.slow()),
+    pytest.param("isl", marks=pytest.mark.slow()),
     pytest.param("kn", marks=pytest.mark.slow()),
     pytest.param("lb", marks=pytest.mark.slow()),
     pytest.param("lt", marks=pytest.mark.slow()),
     pytest.param("lv", marks=pytest.mark.slow()),
     pytest.param("nb", marks=pytest.mark.slow()),
     pytest.param("nl", marks=pytest.mark.slow()),
     "pl",
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/test_naughty_strings.py` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/test_naughty_strings.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/test_tokenizer.py` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/test_urls.py` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/test_urls.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/tokenizer/test_whitespace.py` & `spacy-4.0.0.dev1/spacy/tests/tokenizer/test_whitespace.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_augmenters.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_augmenters.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_logger.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_logger.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_new_example.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_new_example.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_pretraining.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_pretraining.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from pathlib import Path
 import numpy as np
 import pytest
 import srsly
-from spacy.vocab import Vocab
-from thinc.api import Config
+from thinc.api import Config, get_current_ops
 
+from spacy import util
+from spacy.lang.en import English
+from spacy.training.initialize import init_nlp
+from spacy.training.loop import train
+from spacy.training.pretrain import pretrain
+from spacy.tokens import Doc, DocBin
+from spacy.language import DEFAULT_CONFIG_PRETRAIN_PATH, DEFAULT_CONFIG_PATH
+from spacy.ml.models.multi_task import create_pretrain_vectors
+from spacy.vectors import Vectors
+from spacy.vocab import Vocab
 from ..util import make_tempdir
-from ... import util
-from ...lang.en import English
-from ...training.initialize import init_nlp
-from ...training.loop import train
-from ...training.pretrain import pretrain
-from ...tokens import Doc, DocBin
-from ...language import DEFAULT_CONFIG_PRETRAIN_PATH, DEFAULT_CONFIG_PATH
 
 pretrain_string_listener = """
 [nlp]
 lang = "en"
 pipeline = ["tok2vec", "tagger"]
 
 [components]
@@ -159,31 +161,36 @@
     filled = nlp.config
     pretrain_config = util.load_config(DEFAULT_CONFIG_PRETRAIN_PATH)
     filled = pretrain_config.merge(filled)
     assert "PretrainCharacters" in filled["pretraining"]["objective"]["@architectures"]
 
 
 @pytest.mark.parametrize("objective", CHAR_OBJECTIVES)
-def test_pretraining_tok2vec_characters(objective):
+@pytest.mark.parametrize("skip_last", (True, False))
+def test_pretraining_tok2vec_characters(objective, skip_last):
     """Test that pretraining works with the character objective"""
     config = Config().from_str(pretrain_string_listener)
     config["pretraining"]["objective"] = objective
     nlp = util.load_model_from_config(config, auto_fill=True, validate=False)
     filled = nlp.config
     pretrain_config = util.load_config(DEFAULT_CONFIG_PRETRAIN_PATH)
     filled = pretrain_config.merge(filled)
     with make_tempdir() as tmp_dir:
         file_path = write_sample_jsonl(tmp_dir)
         filled["paths"]["raw_text"] = file_path
         filled = filled.interpolate()
         assert filled["pretraining"]["component"] == "tok2vec"
-        pretrain(filled, tmp_dir)
+        pretrain(filled, tmp_dir, skip_last=skip_last)
         assert Path(tmp_dir / "model0.bin").exists()
         assert Path(tmp_dir / "model4.bin").exists()
         assert not Path(tmp_dir / "model5.bin").exists()
+        if skip_last:
+            assert not Path(tmp_dir / "model-last.bin").exists()
+        else:
+            assert Path(tmp_dir / "model-last.bin").exists()
 
 
 @pytest.mark.parametrize("objective", VECTOR_OBJECTIVES)
 def test_pretraining_tok2vec_vectors_fail(objective):
     """Test that pretraining doesn't works with the vectors objective if there are no static vectors"""
     config = Config().from_str(pretrain_string_listener)
     config["pretraining"]["objective"] = objective
@@ -231,14 +238,15 @@
         filled["paths"]["raw_text"] = file_path
         filled["pretraining"]["component"] = "tagger"
         filled["pretraining"]["layer"] = "tok2vec"
         filled = filled.interpolate()
         pretrain(filled, tmp_dir)
         assert Path(tmp_dir / "model0.bin").exists()
         assert Path(tmp_dir / "model4.bin").exists()
+        assert Path(tmp_dir / "model-last.bin").exists()
         assert not Path(tmp_dir / "model5.bin").exists()
 
 
 def test_pretraining_tagger():
     """Test pretraining of the tagger itself will throw an error (not an appropriate tok2vec layer)"""
     config = Config().from_str(pretrain_string_internal)
     nlp = util.load_model_from_config(config, auto_fill=True, validate=False)
@@ -342,7 +350,30 @@
     }
     for word, vector in vector_data.items():
         vocab.set_vector(word, vector)
     nlp_path = tmp_dir / "vectors_model"
     nlp = English(vocab)
     nlp.to_disk(nlp_path)
     return str(nlp_path)
+
+
+def test_pretrain_default_vectors():
+    nlp = English()
+    nlp.add_pipe("tok2vec")
+    nlp.initialize()
+
+    # default vectors are supported
+    nlp.vocab.vectors = Vectors(shape=(10, 10))
+    create_pretrain_vectors(1, 1, "cosine")(nlp.vocab, nlp.get_pipe("tok2vec").model)
+
+    # floret vectors are supported
+    nlp.vocab.vectors = Vectors(
+        data=get_current_ops().xp.zeros((10, 10)), mode="floret", hash_count=1
+    )
+    create_pretrain_vectors(1, 1, "cosine")(nlp.vocab, nlp.get_pipe("tok2vec").model)
+
+    # error for no vectors
+    with pytest.raises(ValueError, match="E875"):
+        nlp.vocab.vectors = Vectors()
+        create_pretrain_vectors(1, 1, "cosine")(
+            nlp.vocab, nlp.get_pipe("tok2vec").model
+        )
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_readers.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_readers.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_rehearse.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_rehearse.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/training/test_training.py` & `spacy-4.0.0.dev1/spacy/tests/training/test_training.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/util.py` & `spacy-4.0.0.dev1/spacy/tests/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy
 import tempfile
 import contextlib
+import re
 import srsly
 from spacy.tokens import Doc
 from spacy.vocab import Vocab
 from spacy.util import make_tempdir  # noqa: F401
 from spacy.training import split_bilu_label
 from thinc.api import get_current_ops
 
@@ -91,7 +92,11 @@
     """Assert that two packed msgpack messages are equal."""
     msg1 = srsly.msgpack_loads(b1)
     msg2 = srsly.msgpack_loads(b2)
     assert sorted(msg1.keys()) == sorted(msg2.keys())
     for (k1, v1), (k2, v2) in zip(sorted(msg1.items()), sorted(msg2.items())):
         assert k1 == k2
         assert v1 == v2
+
+
+def normalize_whitespace(s):
+    return re.sub(r"\s+", " ", s)
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_lexeme.py` & `spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_lexeme.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """Test Issue #361: Equality of lexemes"""
     assert en_vocab[text1] == en_vocab[text1]
     assert en_vocab[text1] != en_vocab[text2]
 
 
 @pytest.mark.issue(600)
 def test_issue600():
-    vocab = Vocab(tag_map={"NN": {"pos": "NOUN"}})
+    vocab = Vocab()
     doc = Doc(vocab, words=["hello"])
     doc[0].tag_ = "NN"
 
 
 @pytest.mark.parametrize("text1,prob1,text2,prob2", [("NOUN", -1, "opera", -2)])
 def test_vocab_lexeme_lt(en_vocab, text1, text2, prob1, prob2):
     """More frequent is l.t. less frequent"""
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_lookups.py` & `spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_lookups.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_similarity.py` & `spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_similarity.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_stringstore.py` & `spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_stringstore.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_vectors.py` & `spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,31 +80,30 @@
     v = Vectors(shape=(10, 10), keys=[5, 3, 98, 100])
     v.resize((100, 100))
 
 
 @pytest.mark.issue(1807)
 def test_issue1807():
     """Test vocab.set_vector also adds the word to the vocab."""
-    vocab = Vocab(vectors_name="test_issue1807")
+    vocab = Vocab()
     assert "hello" not in vocab
     vocab.set_vector("hello", numpy.ones((50,), dtype="f"))
     assert "hello" in vocab
 
 
 @pytest.mark.issue(2871)
 def test_issue2871():
     """Test that vectors recover the correct key for spaCy reserved words."""
     words = ["dog", "cat", "SUFFIX"]
-    vocab = Vocab(vectors_name="test_issue2871")
+    vocab = Vocab()
     vocab.vectors.resize(shape=(3, 10))
     vector_data = numpy.zeros((3, 10), dtype="f")
     for word in words:
         _ = vocab[word]  # noqa: F841
         vocab.set_vector(word, vector_data[0])
-    vocab.vectors.name = "dummy_vectors"
     assert vocab["dog"].rank == 0
     assert vocab["cat"].rank == 1
     assert vocab["SUFFIX"].rank == 2
     assert vocab.vectors.find(key="dog") == 0
     assert vocab.vectors.find(key="cat") == 1
     assert vocab.vectors.find(key="SUFFIX") == 2
 
@@ -121,15 +120,15 @@
 
 @pytest.mark.issue(4725)
 def test_issue4725_2():
     if isinstance(get_current_ops, NumpyOps):
         # ensures that this runs correctly and doesn't hang or crash because of the global vectors
         # if it does crash, it's usually because of calling 'spawn' for multiprocessing (e.g. on Windows),
         # or because of issues with pickling the NER (cf test_issue4725_1)
-        vocab = Vocab(vectors_name="test_vocab_add_vector")
+        vocab = Vocab()
         data = numpy.ndarray((5, 3), dtype="f")
         data[0] = 1.0
         data[1] = 2.0
         vocab.set_vector("cat", data[0])
         vocab.set_vector("dog", data[1])
         nlp = English(vocab=vocab)
         nlp.add_pipe("ner")
@@ -336,15 +335,15 @@
     doc1 = Doc(vocab, words=text1)
     doc2 = Doc(vocab, words=text2)
     assert doc1.similarity(doc2) == doc2.similarity(doc1)
     assert -1.0 < doc1.similarity(doc2) < 1.0
 
 
 def test_vocab_add_vector():
-    vocab = Vocab(vectors_name="test_vocab_add_vector")
+    vocab = Vocab()
     data = OPS.xp.ndarray((5, 3), dtype="f")
     data[0] = 1.0
     data[1] = 2.0
     vocab.set_vector("cat", data[0])
     vocab.set_vector("dog", data[1])
     cat = vocab["cat"]
     assert list(cat.vector) == [1.0, 1.0, 1.0]
@@ -352,15 +351,15 @@
     assert list(dog.vector) == [2.0, 2.0, 2.0]
 
     with pytest.raises(ValueError):
         vocab.vectors.add(vocab["hamster"].orth, row=1000000)
 
 
 def test_vocab_prune_vectors():
-    vocab = Vocab(vectors_name="test_vocab_prune_vectors")
+    vocab = Vocab()
     _ = vocab["cat"]  # noqa: F841
     _ = vocab["dog"]  # noqa: F841
     _ = vocab["kitten"]  # noqa: F841
     data = OPS.xp.ndarray((5, 3), dtype="f")
     data[0] = OPS.asarray([1.0, 1.2, 1.1])
     data[1] = OPS.asarray([0.3, 1.3, 1.0])
     data[2] = OPS.asarray([0.9, 1.22, 1.05])
@@ -401,15 +400,15 @@
         row = v.add("D", vector=OPS.asarray([10, 20, 30, 40], dtype="f"))
         row_r = v_r.add("D", vector=OPS.asarray([10, 20, 30, 40], dtype="f"))
         assert row == row_r
         assert_equal(OPS.to_numpy(v.data), OPS.to_numpy(v_r.data))
 
 
 def test_vector_is_oov():
-    vocab = Vocab(vectors_name="test_vocab_is_oov")
+    vocab = Vocab()
     data = OPS.xp.ndarray((5, 3), dtype="f")
     data[0] = 1.0
     data[1] = 2.0
     vocab.set_vector("cat", data[0])
     vocab.set_vector("dog", data[1])
     assert vocab["cat"].is_oov is False
     assert vocab["dog"].is_oov is False
```

### Comparing `spacy-4.0.0.dev0/spacy/tests/vocab_vectors/test_vocab_api.py` & `spacy-4.0.0.dev1/spacy/tests/vocab_vectors/test_vocab_api.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokenizer.pxd` & `spacy-4.0.0.dev1/spacy/tokenizer.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     cdef int _retokenize_special_spans(self, Doc doc, TokenC* tokens,
                                        object span_data)
     cdef int _try_specials_and_cache(self, hash_t key, Doc tokens,
                                      int* has_special,
                                      bint with_special_cases) except -1
     cdef int _tokenize(self, Doc tokens, str span, hash_t key,
                        int* has_special, bint with_special_cases) except -1
-    cdef str _split_affixes(self, Pool mem, str string,
+    cdef str _split_affixes(self, str string,
                                 vector[LexemeC*] *prefixes,
                                 vector[LexemeC*] *suffixes, int* has_special,
                                 bint with_special_cases)
     cdef int _attach_tokens(self, Doc tokens, str string,
                             vector[LexemeC*] *prefixes,
                             vector[LexemeC*] *suffixes, int* has_special,
                             bint with_special_cases) except -1
```

### Comparing `spacy-4.0.0.dev0/spacy/tokenizer.pyx` & `spacy-4.0.0.dev1/spacy/tokenizer.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -385,22 +385,22 @@
         return True
 
     cdef int _tokenize(self, Doc tokens, str span, hash_t orig_key, int* has_special, bint with_special_cases) except -1:
         cdef vector[LexemeC*] prefixes
         cdef vector[LexemeC*] suffixes
         cdef int orig_size
         orig_size = tokens.length
-        span = self._split_affixes(tokens.mem, span, &prefixes, &suffixes,
+        span = self._split_affixes(span, &prefixes, &suffixes,
                                    has_special, with_special_cases)
         self._attach_tokens(tokens, span, &prefixes, &suffixes, has_special,
                             with_special_cases)
         self._save_cached(&tokens.c[orig_size], orig_key, has_special,
                           tokens.length - orig_size)
 
-    cdef str _split_affixes(self, Pool mem, str string,
+    cdef str _split_affixes(self, str string,
                                 vector[const LexemeC*] *prefixes,
                                 vector[const LexemeC*] *suffixes,
                                 int* has_special,
                                 bint with_special_cases):
         cdef size_t i
         cdef str prefix
         cdef str suffix
@@ -415,34 +415,34 @@
             last_size = len(string)
             pre_len = self.find_prefix(string)
             if pre_len != 0:
                 prefix = string[:pre_len]
                 minus_pre = string[pre_len:]
                 if minus_pre and with_special_cases and self._specials.get(hash_string(minus_pre)) != NULL:
                     string = minus_pre
-                    prefixes.push_back(self.vocab.get(mem, prefix))
+                    prefixes.push_back(self.vocab.get(prefix))
                     break
             suf_len = self.find_suffix(string[pre_len:])
             if suf_len != 0:
                 suffix = string[-suf_len:]
                 minus_suf = string[:-suf_len]
                 if minus_suf and with_special_cases and self._specials.get(hash_string(minus_suf)) != NULL:
                     string = minus_suf
-                    suffixes.push_back(self.vocab.get(mem, suffix))
+                    suffixes.push_back(self.vocab.get(suffix))
                     break
             if pre_len and suf_len and (pre_len + suf_len) <= len(string):
                 string = string[pre_len:-suf_len]
-                prefixes.push_back(self.vocab.get(mem, prefix))
-                suffixes.push_back(self.vocab.get(mem, suffix))
+                prefixes.push_back(self.vocab.get(prefix))
+                suffixes.push_back(self.vocab.get(suffix))
             elif pre_len:
                 string = minus_pre
-                prefixes.push_back(self.vocab.get(mem, prefix))
+                prefixes.push_back(self.vocab.get(prefix))
             elif suf_len:
                 string = minus_suf
-                suffixes.push_back(self.vocab.get(mem, suffix))
+                suffixes.push_back(self.vocab.get(suffix))
         return string
 
     cdef int _attach_tokens(self, Doc tokens, str string,
                             vector[const LexemeC*] *prefixes,
                             vector[const LexemeC*] *suffixes,
                             int* has_special,
                             bint with_special_cases) except -1:
@@ -461,46 +461,46 @@
                 pass
             elif (self.token_match and self.token_match(string)) or \
                     (self.url_match and \
                     self.url_match(string)):
                 # We're always saying 'no' to spaces here -- the caller will
                 # fix up the outermost one, with reference to the original.
                 # See Issue #859
-                tokens.push_back(self.vocab.get(tokens.mem, string), False)
+                tokens.push_back(self.vocab.get(string), False)
             else:
                 matches = self.find_infix(string)
                 if not matches:
-                    tokens.push_back(self.vocab.get(tokens.mem, string), False)
+                    tokens.push_back(self.vocab.get(string), False)
                 else:
                     # Let's say we have dyn-o-mite-dave - the regex finds the
                     # start and end positions of the hyphens
                     start = 0
                     start_before_infixes = start
                     for match in matches:
                         infix_start = match.start()
                         infix_end = match.end()
 
                         if infix_start == start_before_infixes:
                             continue
 
                         if infix_start != start:
                             span = string[start:infix_start]
-                            tokens.push_back(self.vocab.get(tokens.mem, span), False)
+                            tokens.push_back(self.vocab.get(span), False)
 
                         if infix_start != infix_end:
                             # If infix_start != infix_end, it means the infix
                             # token is non-empty. Empty infix tokens are useful
                             # for tokenization in some languages (see
                             # https://github.com/explosion/spaCy/issues/768)
                             infix_span = string[infix_start:infix_end]
-                            tokens.push_back(self.vocab.get(tokens.mem, infix_span), False)
+                            tokens.push_back(self.vocab.get(infix_span), False)
                         start = infix_end
                     span = string[start:]
                     if span:
-                        tokens.push_back(self.vocab.get(tokens.mem, span), False)
+                        tokens.push_back(self.vocab.get(span), False)
         cdef vector[const LexemeC*].reverse_iterator it = suffixes.rbegin()
         while it != suffixes.rend():
             lexeme = deref(it)
             preinc(it)
             tokens.push_back(lexeme, False)
 
     cdef int _save_cached(self, const TokenC* tokens, hash_t key,
@@ -829,18 +829,20 @@
             self.suffix_search = re.compile(data["suffix_search"]).search
         if "infix_finditer" in data and isinstance(data["infix_finditer"], str):
             self.infix_finditer = re.compile(data["infix_finditer"]).finditer
         if "token_match" in data and isinstance(data["token_match"], str):
             self.token_match = re.compile(data["token_match"]).match
         if "url_match" in data and isinstance(data["url_match"], str):
             self.url_match = re.compile(data["url_match"]).match
-        if "rules" in data and isinstance(data["rules"], dict):
-            self.rules = data["rules"]
         if "faster_heuristics" in data:
             self.faster_heuristics = data["faster_heuristics"]
+        # always load rules last so that all other settings are set before the
+        # internal tokenization for the phrase matcher
+        if "rules" in data and isinstance(data["rules"], dict):
+            self.rules = data["rules"]
         return self
 
 
 def _get_regex_pattern(regex):
     """Get a pattern string for a regex, or None if the pattern is None."""
     return None if regex is None else regex.__self__.pattern
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/doc.pxd` & `spacy-4.0.0.dev1/spacy/tokens/doc.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/doc.pyi` & `spacy-4.0.0.dev1/spacy/tokens/doc.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,19 @@
     @property
     def doc(self) -> Doc: ...
     def char_span(
         self,
         start_idx: int,
         end_idx: int,
         label: Union[int, str] = ...,
+        *,
         kb_id: Union[int, str] = ...,
         vector: Optional[Floats1d] = ...,
         alignment_mode: str = ...,
+        span_id: Union[int, str] = ...,
     ) -> Span: ...
     def similarity(self, other: Union[Doc, Span, Token, Lexeme]) -> float: ...
     @property
     def has_vector(self) -> bool: ...
     vector: Floats1d
     vector_norm: float
     @property
@@ -122,20 +124,20 @@
     def set_ents(
         self,
         entities: List[Span],
         *,
         blocked: Optional[List[Span]] = ...,
         missing: Optional[List[Span]] = ...,
         outside: Optional[List[Span]] = ...,
-        default: str = ...
+        default: str = ...,
     ) -> None: ...
     @property
-    def noun_chunks(self) -> Iterator[Span]: ...
+    def noun_chunks(self) -> Tuple[Span]: ...
     @property
-    def sents(self) -> Iterator[Span]: ...
+    def sents(self) -> Tuple[Span]: ...
     @property
     def lang(self) -> int: ...
     @property
     def lang_(self) -> str: ...
     def count_by(
         self, attr_id: int, exclude: Optional[Any] = ..., counts: Optional[Any] = ...
     ) -> Dict[Any, int]: ...
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/doc.pyx` & `spacy-4.0.0.dev1/spacy/tokens/doc.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -262,20 +262,20 @@
         words = words if words is not None else []
         spaces = spaces if spaces is not None else ([True] * len(words))
         if len(spaces) != len(words):
             raise ValueError(Errors.E027)
         cdef const LexemeC* lexeme
         for word, has_space in zip(words, spaces):
             if isinstance(word, str):
-                lexeme = self.vocab.get(self.mem, word)
+                lexeme = self.vocab.get(word)
             elif isinstance(word, bytes):
                 raise ValueError(Errors.E028.format(value=word))
             else:
                 try:
-                    lexeme = self.vocab.get_by_orth(self.mem, word)
+                    lexeme = self.vocab.get_by_orth(word)
                 except TypeError:
                     raise TypeError(Errors.E1022.format(wtype=type(word)))
             self.push_back(lexeme, has_space)
 
         if heads is not None:
             heads = [head - i if head is not None else 0 for i, head in enumerate(heads)]
         if deps is not None:
@@ -516,41 +516,38 @@
     def __repr__(self):
         return self.__str__()
 
     @property
     def doc(self):
         return self
 
-    def char_span(self, int start_idx, int end_idx, label=0, kb_id=0, vector=None, alignment_mode="strict", span_id=0):
+    def char_span(self, int start_idx, int end_idx, label=0, *, kb_id=0, vector=None, alignment_mode="strict", span_id=0):
         """Create a `Span` object from the slice
         `doc.text[start_idx : end_idx]`. Returns None if no valid `Span` can be
         created.
 
         doc (Doc): The parent document.
         start_idx (int): The index of the first character of the span.
         end_idx (int): The index of the first character after the span.
-        label (uint64 or string): A label to attach to the Span, e.g. for
+        label (Union[int, str]): A label to attach to the Span, e.g. for
             named entities.
-        kb_id (uint64 or string):  An ID from a KB to capture the meaning of a
+        kb_id (Union[int, str]):  An ID from a KB to capture the meaning of a
             named entity.
         vector (ndarray[ndim=1, dtype='float32']): A meaning representation of
             the span.
         alignment_mode (str): How character indices are aligned to token
             boundaries. Options: "strict" (character indices must be aligned
             with token boundaries), "contract" (span of all tokens completely
             within the character span), "expand" (span of all tokens at least
             partially covered by the character span). Defaults to "strict".
+        span_id (Union[int, str]): An identifier to associate with the span.
         RETURNS (Span): The newly constructed object.
 
         DOCS: https://spacy.io/api/doc#char_span
         """
-        if not isinstance(label, int):
-            label = self.vocab.strings.add(label)
-        if not isinstance(kb_id, int):
-            kb_id = self.vocab.strings.add(kb_id)
         alignment_modes = ("strict", "contract", "expand")
         if alignment_mode not in alignment_modes:
             raise ValueError(
                 Errors.E202.format(
                     name="alignment",
                     mode=alignment_mode,
                     modes=", ".join(alignment_modes),
@@ -652,17 +649,14 @@
             xp = get_array_module(self.vocab.vectors.data)
             if not len(self):
                 self._vector = xp.zeros((self.vocab.vectors_length,), dtype="f")
                 return self._vector
             elif self.vocab.vectors.size > 0:
                 self._vector = sum(t.vector for t in self) / len(self)
                 return self._vector
-            elif self.tensor.size > 0:
-                self._vector = self.tensor.mean(axis=0)
-                return self._vector
             else:
                 return xp.zeros((self.vocab.vectors_length,), dtype="float32")
 
         def __set__(self, value):
             self._vector = value
 
     property vector_norm:
@@ -701,18 +695,18 @@
         `Span` and `Token`.
 
         RETURNS (str): The original verbatim text of the document.
         """
         return self.text
 
     property ents:
-        """The named entities in the document. Returns a tuple of named entity
+        """The named entities in the document. Returns a list of named entity
         `Span` objects, if the entity recognizer has been applied.
 
-        RETURNS (tuple): Entities in the document, one `Span` per entity.
+        RETURNS (Tuple[Span]): Entities in the document, one `Span` per entity.
 
         DOCS: https://spacy.io/api/doc#ents
         """
         def __get__(self):
             cdef int i
             cdef const TokenC* token
             cdef int start = -1
@@ -862,53 +856,52 @@
         Raises a NotImplementedError otherwise.
 
         A base noun phrase, or "NP chunk", is a noun
         phrase that does not permit other NPs to be nested within it – so no
         NP-level coordination, no prepositional phrases, and no relative
         clauses.
 
-        YIELDS (Span): Noun chunks in the document.
+        RETURNS (Tuple[Span]): Noun chunks in the document.
 
         DOCS: https://spacy.io/api/doc#noun_chunks
         """
         if self.noun_chunks_iterator is None:
             raise NotImplementedError(Errors.E894.format(lang=self.vocab.lang))
 
         # Accumulate the result before beginning to iterate over it. This
         # prevents the tokenization from being changed out from under us
-        # during the iteration. The tricky thing here is that Span accepts
-        # its tokenization changing, so it's okay once we have the Span
-        # objects. See Issue #375.
+        # during the iteration.
         spans = []
         for start, end, label in self.noun_chunks_iterator(self):
             spans.append(Span(self, start, end, label=label))
-        for span in spans:
-            yield span
+        return tuple(spans)
 
     @property
     def sents(self):
         """Iterate over the sentences in the document. Yields sentence `Span`
         objects. Sentence spans have no label.
 
-        YIELDS (Span): Sentences in the document.
+        RETURNS (Tuple[Span]): Sentences in the document.
 
         DOCS: https://spacy.io/api/doc#sents
         """
         if not self.has_annotation("SENT_START"):
             raise ValueError(Errors.E030)
         if "sents" in self.user_hooks:
-            yield from self.user_hooks["sents"](self)
+            return tuple(self.user_hooks["sents"](self))
         else:
             start = 0
+            spans = []
             for i in range(1, self.length):
                 if self.c[i].sent_start == 1:
-                    yield Span(self, start, i)
+                    spans.append(Span(self, start, i))
                     start = i
             if start != self.length:
-                yield Span(self, start, self.length)
+                spans.append(Span(self, start, self.length))
+            return tuple(spans)
 
     @property
     def lang(self):
         """RETURNS (uint64): ID of the language of the doc's vocabulary."""
         return self.vocab.strings[self.vocab.lang]
 
     @property
@@ -1281,20 +1274,22 @@
         other.user_data = copy.deepcopy(self.user_data)
         other.has_unknown_spaces = self.has_unknown_spaces
         other.user_hooks = dict(self.user_hooks)
         other.user_token_hooks = dict(self.user_token_hooks)
         other.user_span_hooks = dict(self.user_span_hooks)
         other.length = self.length
         other.max_length = self.max_length
-        other.spans = self.spans.copy(doc=other)
         buff_size = other.max_length + (PADDING*2)
         assert buff_size > 0
         tokens = <TokenC*>other.mem.alloc(buff_size, sizeof(TokenC))
         memcpy(tokens, self.c - PADDING, buff_size * sizeof(TokenC))
         other.c = &tokens[PADDING]
+        # copy spans after setting tokens so that SpanGroup.copy can verify
+        # that the start/end offsets are valid
+        other.spans = self.spans.copy(doc=other)
         return other
 
     def to_disk(self, path, *, exclude=tuple()):
         """Save the current state to a directory.
 
         path (str / Path): A path to a directory, which will be created if
             it doesn't exist. Paths may be either strings or Path-like objects.
@@ -1363,14 +1358,18 @@
             strings.add(token.ent_type_)
             strings.add(token.ent_kb_id_)
             strings.add(token.ent_id_)
             strings.add(token.norm_)
         for group in self.spans.values():
             for span in group:
                 strings.add(span.label_)
+                if span.kb_id in span.doc.vocab.strings:
+                    strings.add(span.kb_id_)
+                if span.id in span.doc.vocab.strings:
+                    strings.add(span.id_)
         # Msgpack doesn't distinguish between lists and tuples, which is
         # vexing for user data. As a best guess, we *know* that within
         # keys, we must have tuples. In values we just have to hope
         # users don't mind getting a list instead of a tuple.
         serializers = {
             "text": lambda: self.text,
             "array_head": lambda: array_head,
@@ -1426,15 +1425,15 @@
         cdef str orth_
         text = msg["text"]
         attrs = msg["array_body"]
         for i in range(attrs.shape[0]):
             end = start + attrs[i, 0]
             has_space = attrs[i, 1]
             orth_ = text[start:end]
-            lex = self.vocab.get(self.mem, orth_)
+            lex = self.vocab.get(orth_)
             self.push_back(lex, has_space)
             start = end + has_space
         self.from_array(msg["array_head"][2:], attrs[:, 2:])
         if "spans" in msg:
             self.spans.from_bytes(msg["spans"])
         else:
             self.spans.clear()
@@ -1532,15 +1531,15 @@
         start = 0
         cdef const LexemeC* lex
         cdef bint has_space
         reconstructed_words, spaces = get_words_and_spaces(words, doc_json["text"])
         assert words == reconstructed_words
 
         for word, has_space in zip(words, spaces):
-            lex = self.vocab.get(self.mem, word)
+            lex = self.vocab.get(word)
             self.push_back(lex, has_space)
 
         # Set remaining token-level attributes via Doc.from_array().
         if HEAD in token_annotations:
             token_annotations[HEAD] = [
                 head - i for i, head in enumerate(token_annotations[HEAD])
             ]
@@ -1600,15 +1599,15 @@
                 for token in char_span[1:]:
                     token.is_sent_start = False
 
 
         for span_group in doc_json.get("spans", {}):
             spans = []
             for span in doc_json["spans"][span_group]:
-                char_span = self.char_span(span["start"], span["end"], span["label"], span["kb_id"])
+                char_span = self.char_span(span["start"], span["end"], span["label"], kb_id=span["kb_id"])
                 if char_span is None:
                     raise ValueError(Errors.E1039.format(obj="span", start=span["start"], end=span["end"]))
                 spans.append(char_span)
             self.spans[span_group] = spans
 
         if "ents" in doc_json:
             ents = []
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/doc_bin.py` & `spacy-4.0.0.dev1/spacy/tokens/doc_bin.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,18 @@
         self.cats.append(doc.cats)
         if self.store_user_data:
             self.user_data.append(srsly.msgpack_dumps(doc.user_data))
         self.span_groups.append(doc.spans.to_bytes())
         for key, group in doc.spans.items():
             for span in group:
                 self.strings.add(span.label_)
+                if span.kb_id in span.doc.vocab.strings:
+                    self.strings.add(span.kb_id_)
+                if span.id in span.doc.vocab.strings:
+                    self.strings.add(span.id_)
 
     def get_docs(self, vocab: Vocab) -> Iterator[Doc]:
         """Recover Doc objects from the annotations, using the given vocab.
         Note that the user data of each doc will be read (if available) and returned,
         regardless of the setting of 'self.store_user_data'.
 
         vocab (Vocab): The shared vocab.
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/graph.pyx` & `spacy-4.0.0.dev1/spacy/tokens/graph.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/morphanalysis.pyi` & `spacy-4.0.0.dev1/spacy/tokens/morphanalysis.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Dict, Iterator, List, Union
+from typing import Any, Dict, Iterator, List, Optional, Union
 from ..vocab import Vocab
 
 class MorphAnalysis:
     def __init__(
         self, vocab: Vocab, features: Union[Dict[str, str], str] = ...
     ) -> None: ...
     @classmethod
     def from_id(cls, vocab: Vocab, key: Any) -> MorphAnalysis: ...
     def __contains__(self, feature: str) -> bool: ...
     def __iter__(self) -> Iterator[str]: ...
     def __len__(self) -> int: ...
     def __hash__(self) -> int: ...
     def __eq__(self, other: MorphAnalysis) -> bool: ...  # type: ignore[override]
     def __ne__(self, other: MorphAnalysis) -> bool: ...  # type: ignore[override]
-    def get(self, field: Any) -> List[str]: ...
+    def get(self, field: Any, default: Optional[List[str]]) -> List[str]: ...
     def to_json(self) -> str: ...
     def to_dict(self) -> Dict[str, str]: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/morphanalysis.pyx` & `spacy-4.0.0.dev1/spacy/tokens/morphanalysis.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,22 @@
         if isinstance(other, str):
             raise ValueError(Errors.E977)
         return self.key == other.key
 
     def __ne__(self, other):
         return self.key != other.key
 
-    def get(self, field):
+    def get(self, field, default=None):
         """Retrieve feature values by field."""
         cdef attr_t field_id = self.vocab.strings.as_int(field)
         cdef np.ndarray results = get_by_field(self.c, field_id)
+        if len(results) == 0:
+            if default is None:
+                default = []
+            return default
         features = [self.vocab.strings[result] for result in results]
         return [f.split(Morphology.FIELD_SEP)[1] for f in features]
 
     def to_json(self):
         """Produce a json serializable representation as a UD FEATS-style
         string.
         """
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/retokenizer.pyi` & `spacy-4.0.0.dev1/spacy/tokens/retokenizer.pyi`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/retokenizer.pyx` & `spacy-4.0.0.dev1/spacy/tokens/retokenizer.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         if spans[token_index][-1].whitespace_:
             new_orth = new_orth[:-len(spans[token_index][-1].whitespace_)]
         # add the vector of the (merged) entity to the vocab
         if not doc.vocab.get_vector(new_orth).any():
             if doc.vocab.vectors_length > 0:
                 doc.vocab.set_vector(new_orth, span.vector)
         token = tokens[token_index]
-        lex = doc.vocab.get(doc.mem, new_orth)
+        lex = doc.vocab.get(new_orth)
         token.lex = lex
         # We set trailing space here too
         token.spacy = doc.c[spans[token_index].end-1].spacy
         set_token_attrs(span[0], attributes)
     # Begin by setting all the head indices to absolute token positions
     # This is easier to work with for now than the offsets
     # Before thinking of something simpler, beware the case where a
@@ -355,15 +355,15 @@
         doc.c[token_to_move + nb_subtokens - 1] = doc.c[token_to_move]
         if to_process_tensor:
             doc.tensor[token_to_move + nb_subtokens - 1] = doc.tensor[token_to_move]
     # Host the tokens in the newly created space
     cdef int idx_offset = 0
     for i, orth in enumerate(orths):
         token = &doc.c[token_index + i]
-        lex = doc.vocab.get(doc.mem, orth)
+        lex = doc.vocab.get(orth)
         token.lex = lex
         # If lemma is currently set, set default lemma to orth
         if token.lemma != 0:
             token.lemma = lex.orth
         token.norm = 0  # reset norm
         if to_process_tensor:
             # setting the tensors of the split tokens to array of zeros
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/span.pxd` & `spacy-4.0.0.dev1/spacy/tokens/span.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/span.pyi` & `spacy-4.0.0.dev1/spacy/tokens/span.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Callable, Protocol, Iterator, Optional, Union, Tuple, Any, overload
-from thinc.types import Floats1d, Ints2d, FloatsXd
+from typing import Any, Callable, Iterator, Optional, Protocol, Tuple, Union, overload
+
+from thinc.types import Floats1d, FloatsXd, Ints2d
+
+from ..lexeme import Lexeme
+from ..vocab import Vocab
 from .doc import Doc
 from .token import Token
 from .underscore import Underscore
-from ..lexeme import Lexeme
-from ..vocab import Vocab
 
 class SpanMethod(Protocol):
     def __call__(self: Span, *args: Any, **kwargs: Any) -> Any: ...  # type: ignore[misc]
 
 class Span:
     @classmethod
     def set_extension(
@@ -47,15 +49,20 @@
         end: int,
         label: Union[str, int] = ...,
         vector: Optional[Floats1d] = ...,
         vector_norm: Optional[float] = ...,
         kb_id: Union[str, int] = ...,
         span_id: Union[str, int] = ...,
     ) -> None: ...
-    def __richcmp__(self, other: Span, op: int) -> bool: ...
+    def __lt__(self, other: Any) -> bool: ...
+    def __le__(self, other: Any) -> bool: ...
+    def __eq__(self, other: Any) -> bool: ...
+    def __ne__(self, other: Any) -> bool: ...
+    def __gt__(self, other: Any) -> bool: ...
+    def __ge__(self, other: Any) -> bool: ...
     def __hash__(self) -> int: ...
     def __len__(self) -> int: ...
     def __repr__(self) -> str: ...
     @overload
     def __getitem__(self, i: int) -> Token: ...
     @overload
     def __getitem__(self, i: slice) -> Span: ...
@@ -70,36 +77,41 @@
     @property
     def vocab(self) -> Vocab: ...
     @property
     def sent(self) -> Span: ...
     @property
     def ents(self) -> Tuple[Span]: ...
     @property
+    def sents(self) -> Tuple[Span]: ...
+    @property
     def has_vector(self) -> bool: ...
     @property
     def vector(self) -> Floats1d: ...
     @property
     def vector_norm(self) -> float: ...
     @property
     def tensor(self) -> FloatsXd: ...
     @property
     def text(self) -> str: ...
     @property
     def text_with_ws(self) -> str: ...
     @property
-    def noun_chunks(self) -> Iterator[Span]: ...
+    def noun_chunks(self) -> Tuple[Span]: ...
     @property
     def root(self) -> Token: ...
     def char_span(
         self,
         start_idx: int,
         end_idx: int,
         label: Union[int, str] = ...,
+        *,
         kb_id: Union[int, str] = ...,
         vector: Optional[Floats1d] = ...,
+        alignment_mode: str = ...,
+        span_id: Union[int, str] = ...,
     ) -> Span: ...
     @property
     def conjuncts(self) -> Tuple[Token]: ...
     @property
     def lefts(self) -> Iterator[Token]: ...
     @property
     def rights(self) -> Iterator[Token]: ...
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/span.pyx` & `spacy-4.0.0.dev1/spacy/tokens/span.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -130,18 +130,16 @@
     def __richcmp__(self, Span other, int op):
         if other is None:
             if op == 0 or op == 1 or op == 2:
                 return False
             else:
                 return True
 
-        cdef SpanC* span_c = self.span_c()
-        cdef SpanC* other_span_c = other.span_c()
-        self_tuple = (span_c.start_char, span_c.end_char, span_c.label, span_c.kb_id, self.id, self.doc)
-        other_tuple = (other_span_c.start_char, other_span_c.end_char, other_span_c.label, other_span_c.kb_id, other.id, other.doc)
+        self_tuple = self._cmp_tuple()
+        other_tuple = other._cmp_tuple()
         # <
         if op == 0:
             return self_tuple < other_tuple
         # <=
         elif op == 1:
             return self_tuple <= other_tuple
         # ==
@@ -154,16 +152,28 @@
         elif op == 4:
             return self_tuple > other_tuple
         # >=
         elif op == 5:
             return self_tuple >= other_tuple
 
     def __hash__(self):
+        return hash(self._cmp_tuple())
+
+    def _cmp_tuple(self):
         cdef SpanC* span_c = self.span_c()
-        return hash((self.doc, span_c.start_char, span_c.end_char, span_c.label, span_c.kb_id, span_c.id))
+        return (
+            span_c.start_char,
+            span_c.end_char,
+            span_c.start,
+            span_c.end,
+            span_c.label,
+            span_c.kb_id,
+            span_c.id,
+            self.doc,
+        )
 
     def __len__(self):
         """Get the number of tokens in the span.
 
         RETURNS (int): The number of tokens in the span.
 
         DOCS: https://spacy.io/api/span#len
@@ -378,15 +388,15 @@
                 warnings.warn(Warnings.W008.format(obj="Span"))
             return 0.0
         vector = self.vector
         xp = get_array_module(vector)
         result = xp.dot(vector, other.vector) / (self.vector_norm * other.vector_norm)
         # ensure we get a scalar back (numpy does this automatically but cupy doesn't)
         return result.item()
-    
+
     cpdef np.ndarray to_array(self, object py_attr_ids):
         """Given a list of M attribute IDs, export the tokens to a numpy
         `ndarray` of shape `(N, M)`, where `N` is the length of the document.
         The values will be 32-bit integers.
 
         attr_ids (list[int]): A list of attribute ID ints.
         RETURNS (numpy.ndarray[long, ndim=2]): A feature matrix, with one row
@@ -447,87 +457,90 @@
         return self.c.get()
 
     @property
     def sents(self):
         """Obtain the sentences that contain this span. If the given span
         crosses sentence boundaries, return all sentences it is a part of.
 
-        RETURNS (Iterable[Span]): All sentences that the span is a part of.
+        RETURNS (Tuple[Span]): All sentences that the span is a part of.
 
-         DOCS: https://spacy.io/api/span#sents
+        DOCS: https://spacy.io/api/span#sents
         """
         cdef int start
         cdef int i
 
         if "sents" in self.doc.user_span_hooks:
-            yield from self.doc.user_span_hooks["sents"](self)
-        elif "sents" in self.doc.user_hooks:
+            return tuple(self.doc.user_span_hooks["sents"](self))
+        spans = []
+        if "sents" in self.doc.user_hooks:
             for sentence in self.doc.user_hooks["sents"](self.doc):
                 if sentence.end > self.start:
                     if sentence.start < self.end or sentence.start == self.start == self.end:
-                        yield sentence
+                        spans.append(sentence)
                     else:
                         break
         else:
             if not self.doc.has_annotation("SENT_START"):
                 raise ValueError(Errors.E030)
             # Use `sent_start` token attribute to find sentence boundaries
             # Find start of the 1st sentence of the Span
             start = self.start
             while self.doc.c[start].sent_start != 1 and start > 0:
                 start -= 1
 
             # Now, find all the sentences in the span
             for i in range(start + 1, self.doc.length):
                 if self.doc.c[i].sent_start == 1:
-                    yield Span(self.doc, start, i)
+                    spans.append(Span(self.doc, start, i))
                     start = i
                     if start >= self.end:
                         break
-            if start < self.end:
-                yield Span(self.doc, start, self.end)
+                elif i == self.doc.length - 1:
+                    spans.append(Span(self.doc, start, self.doc.length))
 
+            # Ensure that trailing parts of the Span instance are included in last element of .sents.
+            if start == self.doc.length - 1:
+                spans.append(Span(self.doc, start, self.doc.length))
+        return tuple(spans)
 
     @property
     def ents(self):
         """The named entities that fall completely within the span. Returns
         a tuple of `Span` objects.
 
-        RETURNS (tuple): Entities in the span, one `Span` per entity.
+        RETURNS (Tuple[Span]): Entities in the span, one `Span` per entity.
 
         DOCS: https://spacy.io/api/span#ents
         """
         cdef Span ent
         cdef SpanC* span_c = self.span_c()
         cdef SpanC* ent_span_c
         ents = []
         for ent in self.doc.ents:
             ent_span_c = ent.span_c()
             if ent_span_c.start >= span_c.start:
                 if ent_span_c.end <= span_c.end:
                     ents.append(ent)
                 else:
                     break
-        return ents
+        return tuple(ents)
 
     @property
     def has_vector(self):
         """A boolean value indicating whether a word vector is associated with
         the object.
 
         RETURNS (bool): Whether a word vector is associated with the object.
 
         DOCS: https://spacy.io/api/span#has_vector
         """
         if "has_vector" in self.doc.user_span_hooks:
             return self.doc.user_span_hooks["has_vector"](self)
         elif self.vocab.vectors.size > 0:
             return any(token.has_vector for token in self)
-        elif self.doc.tensor.size > 0:
-            return True
         else:
             return False
 
     @property
     def vector(self):
         """A real-valued meaning representation. Defaults to an average of the
         token vectors.
@@ -601,21 +614,23 @@
         Raises a NotImplementedError otherwise.
 
         A base noun phrase, or "NP chunk", is a noun
         phrase that does not permit other NPs to be nested within it – so no
         NP-level coordination, no prepositional phrases, and no relative
         clauses.
 
-        YIELDS (Span): Noun chunks in the span.
+        RETURNS (Tuple[Span]): Noun chunks in the span.
 
         DOCS: https://spacy.io/api/span#noun_chunks
         """
+        spans = []
         for span in self.doc.noun_chunks:
             if span.start >= self.start and span.end <= self.end:
-                yield span
+                spans.append(span)
+        return tuple(spans)
 
     @property
     def root(self):
         """The token with the shortest path to the root of the
         sentence (or the root itself). If multiple tokens are equally
         high in the tree, the first token is taken.
 
@@ -652,30 +667,36 @@
                 current_best = words_to_root
                 root = i
         if root == -1:
             return self.doc[span_c.start]
         else:
             return self.doc[root]
 
-    def char_span(self, int start_idx, int end_idx, label=0, kb_id=0, vector=None, id=0):
+    def char_span(self, int start_idx, int end_idx, label=0, *, kb_id=0, vector=None, alignment_mode="strict", span_id=0):
         """Create a `Span` object from the slice `span.text[start : end]`.
 
-        start (int): The index of the first character of the span.
-        end (int): The index of the first character after the span.
-        label (uint64 or string): A label to attach to the Span, e.g. for
+        start_idx (int): The index of the first character of the span.
+        end_idx (int): The index of the first character after the span.
+        label (Union[int, str]): A label to attach to the Span, e.g. for
             named entities.
-        kb_id (uint64 or string):  An ID from a KB to capture the meaning of a named entity.
+        kb_id (Union[int, str]):  An ID from a KB to capture the meaning of a named entity.
         vector (ndarray[ndim=1, dtype='float32']): A meaning representation of
             the span.
+        alignment_mode (str): How character indices are aligned to token
+            boundaries. Options: "strict" (character indices must be aligned
+            with token boundaries), "contract" (span of all tokens completely
+            within the character span), "expand" (span of all tokens at least
+            partially covered by the character span). Defaults to "strict".
+        span_id (Union[int, str]): An identifier to associate with the span.
         RETURNS (Span): The newly constructed object.
         """
         cdef SpanC* span_c = self.span_c()
         start_idx += span_c.start_char
         end_idx += span_c.start_char
-        return self.doc.char_span(start_idx, end_idx, label=label, kb_id=kb_id, vector=vector)
+        return self.doc.char_span(start_idx, end_idx, label=label, kb_id=kb_id, vector=vector, alignment_mode=alignment_mode, span_id=span_id)
 
     @property
     def conjuncts(self):
         """Tokens that are conjoined to the span's root.
 
         RETURNS (tuple): A tuple of Token objects.
 
@@ -750,44 +771,69 @@
             yield from word.subtree
 
     property start:
         def __get__(self):
             return self.span_c().start
 
         def __set__(self, int start):
-            if start < 0:
-                raise IndexError(Errors.E1032.format(var="start", forbidden="< 0", value=start))
-            self.span_c().start = start
+            if start < 0 or start > self.doc.length:
+                raise IndexError(Errors.E1032.format(var="start", obj="Doc", length=self.doc.length, value=start))
+            cdef SpanC* span_c = self.span_c()
+            if start > span_c.end:
+                raise ValueError(Errors.E4007.format(var="start", value=start, op="<=", existing_var="end", existing_value=span_c.end))
+            span_c.start = start
+            span_c.start_char = self.doc.c[start].idx
 
     property end:
         def __get__(self):
             return self.span_c().end
 
         def __set__(self, int end):
-            if end < 0:
-                raise IndexError(Errors.E1032.format(var="end", forbidden="< 0", value=end))
-            self.span_c().end = end
+            if end < 0 or end > self.doc.length:
+                raise IndexError(Errors.E1032.format(var="end", obj="Doc", length=self.doc.length, value=end))
+            cdef SpanC* span_c = self.span_c()
+            if span_c.start > end:
+                raise ValueError(Errors.E4007.format(var="end", value=end, op=">=", existing_var="start", existing_value=span_c.start))
+            span_c.end = end
+            if end > 0:
+                span_c.end_char = self.doc.c[end-1].idx + self.doc.c[end-1].lex.length
+            else:
+                span_c.end_char = 0
 
     property start_char:
         def __get__(self):
             return self.span_c().start_char
 
         def __set__(self, int start_char):
-            if start_char < 0:
-                raise IndexError(Errors.E1032.format(var="start_char", forbidden="< 0", value=start_char))
-            self.span_c().start_char = start_char
+            if start_char < 0 or start_char > len(self.doc.text):
+                raise IndexError(Errors.E1032.format(var="start_char", obj="Doc text", length=len(self.doc.text), value=start_char))
+            cdef int start = token_by_start(self.doc.c, self.doc.length, start_char)
+            if start < 0:
+                raise ValueError(Errors.E4008.format(value=start_char, pos="start"))
+            cdef SpanC* span_c = self.span_c()
+            if start_char > span_c.end_char:
+                raise ValueError(Errors.E4007.format(var="start_char", value=start_char, op="<=", existing_var="end_char", existing_value=span_c.end_char))
+            span_c.start_char = start_char
+            span_c.start = start
 
     property end_char:
         def __get__(self):
             return self.span_c().end_char
 
         def __set__(self, int end_char):
-            if end_char < 0:
-                raise IndexError(Errors.E1032.format(var="end_char", forbidden="< 0", value=end_char))
-            self.span_c().end_char = end_char
+            if end_char < 0 or end_char > len(self.doc.text):
+                raise IndexError(Errors.E1032.format(var="end_char", obj="Doc text", length=len(self.doc.text), value=end_char))
+            cdef int end = token_by_end(self.doc.c, self.doc.length, end_char)
+            if end < 0:
+                raise ValueError(Errors.E4008.format(value=end_char, pos="end"))
+            cdef SpanC* span_c = self.span_c()
+            if span_c.start_char > end_char:
+                raise ValueError(Errors.E4007.format(var="end_char", value=end_char, op=">=", existing_var="start_char", existing_value=span_c.start_char))
+            span_c.end_char = end_char
+            span_c.end = end
 
     property label:
         def __get__(self):
             return self.span_c().label
 
         def __set__(self, attr_t label):
             if label != self.span_c().label :
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/span_group.pyi` & `spacy-4.0.0.dev1/spacy/tokens/span_group.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, Iterable, Optional
+from typing import Any, Dict, Iterable, Iterator, Optional
+
 from .doc import Doc
 from .span import Span
 
 class SpanGroup:
     name: str
     attrs: Dict[str, Any]
     def __init__(
@@ -14,15 +15,15 @@
         spans: Iterable[Span] = ...
     ) -> None: ...
     def __repr__(self) -> str: ...
     @property
     def doc(self) -> Doc: ...
     @property
     def has_overlap(self) -> bool: ...
-    def __iter__(self): ...
+    def __iter__(self) -> Iterator[Span]: ...
     def __len__(self) -> int: ...
     def append(self, span: Span) -> None: ...
     def extend(self, spans: Iterable[Span]) -> None: ...
     def __getitem__(self, i: int) -> Span: ...
     def to_bytes(self) -> bytes: ...
     def from_bytes(self, bytes_data: bytes) -> SpanGroup: ...
     def copy(self, doc: Optional[Doc] = ...) -> SpanGroup: ...
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/span_group.pyx` & `spacy-4.0.0.dev1/spacy/tokens/span_group.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
         self._doc_ref = weakref.ref(doc)
         self.name = name
         self.attrs = dict(attrs) if attrs is not None else {}
         cdef Span span
         if len(spans) :
             self.c.reserve(len(spans))
         for span in spans:
+            if doc is not span.doc:
+                raise ValueError(Errors.E855.format(obj="span"))
             self.push_back(span.c)
 
     def __repr__(self):
         return str(list(self))
 
     @property
     def doc(self):
@@ -260,19 +262,30 @@
         doc (Doc): New reference document to which the copy is bound.
         RETURNS (SpanGroup): A copy of the span group.
 
         DOCS: https://spacy.io/api/spangroup#copy
         """
         if doc is None:
             doc = self.doc
+        if doc is self.doc:
+            spans = list(self)
+        else:
+            spans = [doc.char_span(span.start_char, span.end_char, label=span.label_, kb_id=span.kb_id, span_id=span.id) for span in self]
+            for i, span in enumerate(spans):
+                if span is None:
+                    raise ValueError(Errors.E1052.format(i=i))
+                if span.kb_id in self.doc.vocab.strings:
+                    doc.vocab.strings.add(span.kb_id_)
+                if span.id in span.doc.vocab.strings:
+                    doc.vocab.strings.add(span.id_)
         return SpanGroup(
             doc,
             name=self.name,
             attrs=deepcopy(self.attrs),
-            spans=list(self),
+            spans=spans,
         )
 
     def _concat(
         self,
         other: Union[SpanGroup, Iterable["Span"]],
         *,
         inplace: bool = False,
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/span_groups.py` & `spacy-4.0.0.dev1/spacy/tokens/span_groups.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/token.pxd` & `spacy-4.0.0.dev1/spacy/tokens/token.pxd`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/token.pyi` & `spacy-4.0.0.dev1/spacy/tokens/token.pyi`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/tokens/token.pyx` & `spacy-4.0.0.dev1/spacy/tokens/token.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -385,31 +385,27 @@
 
         RETURNS (bool): Whether a word vector is associated with the object.
 
         DOCS: https://spacy.io/api/token#has_vector
         """
         if "has_vector" in self.doc.user_token_hooks:
             return self.doc.user_token_hooks["has_vector"](self)
-        if self.vocab.vectors.size == 0 and self.doc.tensor.size != 0:
-            return True
         return self.vocab.has_vector(self.c.lex.orth)
 
     @property
     def vector(self):
         """A real-valued meaning representation.
 
         RETURNS (numpy.ndarray[ndim=1, dtype='float32']): A 1D numpy array
             representing the token's semantics.
 
         DOCS: https://spacy.io/api/token#vector
         """
         if "vector" in self.doc.user_token_hooks:
             return self.doc.user_token_hooks["vector"](self)
-        if self.vocab.vectors.size == 0 and self.doc.tensor.size != 0:
-            return self.doc.tensor[self.i]
         else:
             return self.vocab.get_vector(self.c.lex.orth)
 
     @property
     def vector_norm(self):
         """The L2 norm of the token's vector representation.
```

### Comparing `spacy-4.0.0.dev0/spacy/tokens/underscore.py` & `spacy-4.0.0.dev1/spacy/tokens/underscore.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/__init__.py` & `spacy-4.0.0.dev1/spacy/training/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .corpus import Corpus, JsonlCorpus  # noqa: F401
+from .corpus import Corpus, JsonlCorpus, PlainTextCorpus  # noqa: F401
 from .example import Example, validate_examples, validate_get_examples  # noqa: F401
 from .example import validate_distillation_examples  # noqa: F401
 from .alignment import Alignment  # noqa: F401
 from .augment import dont_augment, orth_variants_augmenter  # noqa: F401
 from .iob_utils import iob_to_biluo, biluo_to_iob  # noqa: F401
 from .iob_utils import offsets_to_biluo_tags, biluo_tags_to_offsets  # noqa: F401
 from .iob_utils import biluo_tags_to_spans, tags_to_entities  # noqa: F401
```

### Comparing `spacy-4.0.0.dev0/spacy/training/align.pyx` & `spacy-4.0.0.dev1/spacy/training/align.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/alignment.py` & `spacy-4.0.0.dev1/spacy/training/alignment.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/alignment_array.pyx` & `spacy-4.0.0.dev1/spacy/training/alignment_array.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/augment.py` & `spacy-4.0.0.dev1/spacy/training/augment.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/batchers.py` & `spacy-4.0.0.dev1/spacy/training/batchers.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/callbacks.py` & `spacy-4.0.0.dev1/spacy/training/callbacks.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 @registry.callbacks("spacy.copy_from_base_model.v1")
 def create_copy_from_base_model(
     tokenizer: Optional[str] = None,
     vocab: Optional[str] = None,
 ) -> Callable[[Language], Language]:
     def copy_from_base_model(nlp):
         if tokenizer:
-            logger.info(f"Copying tokenizer from: {tokenizer}")
+            logger.info("Copying tokenizer from: %s", tokenizer)
             base_nlp = load_model(tokenizer)
             if nlp.config["nlp"]["tokenizer"] == base_nlp.config["nlp"]["tokenizer"]:
                 nlp.tokenizer.from_bytes(base_nlp.tokenizer.to_bytes(exclude=["vocab"]))
             else:
                 raise ValueError(
                     Errors.E872.format(
                         curr_config=nlp.config["nlp"]["tokenizer"],
                         base_config=base_nlp.config["nlp"]["tokenizer"],
                     )
                 )
         if vocab:
-            logger.info(f"Copying vocab from: {vocab}")
+            logger.info("Copying vocab from: %s", vocab)
             # only reload if the vocab is from a different model
             if tokenizer != vocab:
                 base_nlp = load_model(vocab)
             nlp.vocab.from_bytes(base_nlp.vocab.to_bytes())
 
     return copy_from_base_model
```

### Comparing `spacy-4.0.0.dev0/spacy/training/converters/conll_ner_to_docs.py` & `spacy-4.0.0.dev1/spacy/training/converters/conll_ner_to_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             "No document delimiters found. Use `-n` to automatically group "
             "sentences into documents."
         )
 
     if model:
         nlp = load_model(model)
     else:
-        nlp = get_lang_class("xx")()
+        nlp = get_lang_class("mul")()
     for conll_doc in input_data.strip().split(doc_delimiter):
         conll_doc = conll_doc.strip()
         if not conll_doc:
             continue
         words = []
         sent_starts = []
         pos_tags = []
@@ -129,15 +129,15 @@
                     nlp.replace_listeners(name, "parser", ["model.tok2vec"])
             sentencizer = nlp.get_pipe("parser")
     if not sentencizer:
         msg.info(
             "Segmenting sentences with sentencizer. (Use `-b model` for "
             "improved parser-based sentence segmentation.)"
         )
-        nlp = get_lang_class("xx")()
+        nlp = get_lang_class("mul")()
         sentencizer = nlp.create_pipe("sentencizer")
     lines = doc.strip().split("\n")
     words = [line.strip().split()[0] for line in lines]
     nlpdoc = Doc(nlp.vocab, words=words)
     sentencizer(nlpdoc)
     lines_with_segs = []
     sent_count = 0
```

### Comparing `spacy-4.0.0.dev0/spacy/training/converters/conllu_to_docs.py` & `spacy-4.0.0.dev1/spacy/training/converters/conllu_to_docs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/converters/iob_to_docs.py` & `spacy-4.0.0.dev1/spacy/training/converters/iob_to_docs.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/converters/json_to_docs.py` & `spacy-4.0.0.dev1/spacy/training/converters/json_to_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import srsly
 from ..gold_io import json_iterate, json_to_annotations
 from ..example import annotations_to_doc
 from ..example import _fix_legacy_dict_data, _parse_example_dict_data
 from ...util import load_model
-from ...lang.xx import MultiLanguage
+from ...lang.mul import MultiLanguage
 
 
 def json_to_docs(input_data, model=None, **kwargs):
     nlp = load_model(model) if model is not None else MultiLanguage()
     if not isinstance(input_data, bytes):
         if not isinstance(input_data, str):
             input_data = srsly.json_dumps(input_data)
```

### Comparing `spacy-4.0.0.dev0/spacy/training/corpus.py` & `spacy-4.0.0.dev1/spacy/training/corpus.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     gold_preproc: bool,
     max_length: int = 0,
     limit: int = 0,
     augmenter: Optional[Callable] = None,
 ) -> Callable[["Language"], Iterable[Example]]:
     if path is None:
         raise ValueError(Errors.E913)
-    util.logger.debug(f"Loading corpus from path: {path}")
+    util.logger.debug("Loading corpus from path: %s", path)
     return Corpus(
         path,
         gold_preproc=gold_preproc,
         max_length=max_length,
         limit=limit,
         augmenter=augmenter,
     )
@@ -54,14 +54,36 @@
     # I decided not to give this a generic name, because I don't want people to
     # use it for arbitrary stuff, as I want this require arg with default False.
     if not require and not path.exists():
         return None
     return srsly.read_json(path)
 
 
+@util.registry.readers("spacy.PlainTextCorpus.v1")
+def create_plain_text_reader(
+    path: Optional[Path],
+    min_length: int = 0,
+    max_length: int = 0,
+) -> Callable[["Language"], Iterable[Doc]]:
+    """Iterate Example objects from a file or directory of plain text
+    UTF-8 files with one line per doc.
+
+    path (Path): The directory or filename to read from.
+    min_length (int): Minimum document length (in tokens). Shorter documents
+        will be skipped. Defaults to 0, which indicates no limit.
+    max_length (int): Maximum document length (in tokens). Longer documents will
+        be skipped. Defaults to 0, which indicates no limit.
+
+    DOCS: https://spacy.io/api/corpus#plaintextcorpus
+    """
+    if path is None:
+        raise ValueError(Errors.E913)
+    return PlainTextCorpus(path, min_length=min_length, max_length=max_length)
+
+
 def walk_corpus(path: Union[str, Path], file_type) -> List[Path]:
     path = util.ensure_path(path)
     if not path.is_dir() and path.parts[-1].endswith(file_type):
         return [path]
     orig_path = path
     paths = [path]
     locs = []
@@ -253,7 +275,56 @@
                     continue
                 else:
                     words = [w.text for w in doc]
                     spaces = [bool(w.whitespace_) for w in doc]
                     # We don't *need* an example here, but it seems nice to
                     # make it match the Corpus signature.
                     yield Example(doc, Doc(nlp.vocab, words=words, spaces=spaces))
+
+
+class PlainTextCorpus:
+    """Iterate Example objects from a file or directory of plain text
+    UTF-8 files with one line per doc.
+
+    path (Path): The directory or filename to read from.
+    min_length (int): Minimum document length (in tokens). Shorter documents
+        will be skipped. Defaults to 0, which indicates no limit.
+    max_length (int): Maximum document length (in tokens). Longer documents will
+        be skipped. Defaults to 0, which indicates no limit.
+
+    DOCS: https://spacy.io/api/corpus#plaintextcorpus
+    """
+
+    file_type = "txt"
+
+    def __init__(
+        self,
+        path: Optional[Union[str, Path]],
+        *,
+        min_length: int = 0,
+        max_length: int = 0,
+    ) -> None:
+        self.path = util.ensure_path(path)
+        self.min_length = min_length
+        self.max_length = max_length
+
+    def __call__(self, nlp: "Language") -> Iterator[Example]:
+        """Yield examples from the data.
+
+        nlp (Language): The current nlp object.
+        YIELDS (Example): The example objects.
+
+        DOCS: https://spacy.io/api/corpus#plaintextcorpus-call
+        """
+        for loc in walk_corpus(self.path, ".txt"):
+            with open(loc, encoding="utf-8") as f:
+                for text in f:
+                    text = text.rstrip("\r\n")
+                    if len(text):
+                        doc = nlp.make_doc(text)
+                        if self.min_length >= 1 and len(doc) < self.min_length:
+                            continue
+                        elif self.max_length >= 1 and len(doc) > self.max_length:
+                            continue
+                        # We don't *need* an example here, but it seems nice to
+                        # make it match the Corpus signature.
+                        yield Example(doc, doc.copy())
```

### Comparing `spacy-4.0.0.dev0/spacy/training/example.pyx` & `spacy-4.0.0.dev1/spacy/training/example.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/gold_io.pyx` & `spacy-4.0.0.dev1/spacy/training/gold_io.pyx`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/initialize.py` & `spacy-4.0.0.dev1/spacy/training/initialize.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 from typing import Union, Dict, Optional, Any, IO, TYPE_CHECKING
-from thinc.api import Config, fix_random_seed, set_gpu_allocator
-from thinc.api import ConfigValidationError
+from thinc.api import Config, ConfigValidationError
 from pathlib import Path
 import srsly
 import numpy
 import tarfile
 import gzip
 import zipfile
 import tqdm
 from itertools import islice
 import warnings
 
 from .pretrain import get_tok2vec_ref
 from ..lookups import Lookups
 from ..vectors import Vectors, Mode as VectorsMode
 from ..errors import Errors, Warnings
-from ..schemas import ConfigSchemaTraining
+from ..schemas import ConfigSchemaDistill, ConfigSchemaTraining
 from ..util import registry, load_model_from_config, resolve_dot_names, logger
 from ..util import load_model, ensure_path, get_sourced_components
 from ..util import OOV_RANK, DEFAULT_OOV_PROB
+from ..util import set_gpu_allocator_from_config, set_seed_from_config
 
 if TYPE_CHECKING:
     from ..language import Language  # noqa: F401
 
 
 def init_nlp(config: Config, *, use_gpu: int = -1) -> "Language":
     raw_config = config
     config = raw_config.interpolate()
-    if "seed" not in config["training"]:
-        raise ValueError(Errors.E1015.format(value="[training] seed"))
-    if "gpu_allocator" not in config["training"]:
-        raise ValueError(Errors.E1015.format(value="[training] gpu_allocator"))
-    if config["training"]["seed"] is not None:
-        fix_random_seed(config["training"]["seed"])
-    allocator = config["training"]["gpu_allocator"]
-    if use_gpu >= 0 and allocator:
-        set_gpu_allocator(allocator)
+    set_seed_from_config(config)
+    set_gpu_allocator_from_config(config, use_gpu)
     # Use original config here before it's resolved to functions
     sourced = get_sourced_components(config)
     nlp = load_model_from_config(raw_config, auto_fill=True)
     logger.info("Set up nlp object from config")
     config = nlp.config.interpolate()
     # Resolve all training-relevant sections using the filled nlp config
     T = registry.resolve(config["training"], schema=ConfigSchemaTraining)
@@ -58,34 +51,131 @@
         )
     train_corpus, dev_corpus = resolve_dot_names(config, dot_names)
     optimizer = T["optimizer"]
     # Components that shouldn't be updated during training
     frozen_components = T["frozen_components"]
     # Sourced components that require resume_training
     resume_components = [p for p in sourced if p not in frozen_components]
+    logger.info("Pipeline: %s", nlp.pipe_names)
+    if resume_components:
+        with nlp.select_pipes(enable=resume_components):
+            logger.info("Resuming training for: %s", resume_components)
+            nlp.resume_training(sgd=optimizer)
+    # Make sure that listeners are defined before initializing further
+    nlp._link_components()
+    with nlp.select_pipes(disable=[*frozen_components, *resume_components]):
+        if T["max_epochs"] == -1:
+            sample_size = 100
+            logger.debug(
+                "Due to streamed train corpus, using only first %s examples for initialization. "
+                "If necessary, provide all labels in [initialize]. "
+                "More info: https://spacy.io/api/cli#init_labels",
+                sample_size,
+            )
+            nlp.initialize(
+                lambda: islice(train_corpus(nlp), sample_size), sgd=optimizer
+            )
+        else:
+            nlp.initialize(lambda: train_corpus(nlp), sgd=optimizer)
+        logger.info("Initialized pipeline components: %s", nlp.pipe_names)
+    # Detect components with listeners that are not frozen consistently
+    for name, proc in nlp.pipeline:
+        for listener in getattr(
+            proc, "listening_components", []
+        ):  # e.g. tok2vec/transformer
+            # Don't warn about components not in the pipeline
+            if listener not in nlp.pipe_names:
+                continue
+            if listener in frozen_components and name not in frozen_components:
+                logger.warning(Warnings.W087.format(name=name, listener=listener))
+            # We always check this regardless, in case user freezes tok2vec
+            if listener not in frozen_components and name in frozen_components:
+                if name not in T["annotating_components"]:
+                    logger.warning(Warnings.W086.format(name=name, listener=listener))
+    return nlp
+
+
+def init_nlp_student(
+    config: Config, teacher: "Language", *, use_gpu: int = -1
+) -> "Language":
+    """Initialize student pipeline for distillation.
+
+    config (Config): Student model configuration.
+    teacher (Language): The teacher pipeline to distill from.
+    use_gpu (int): Whether to train on GPU. Make sure to call require_gpu
+        before calling this function.
+    """
+    raw_config = config
+    config = raw_config.interpolate()
+    set_seed_from_config(config)
+    set_gpu_allocator_from_config(config, use_gpu)
+
+    # Use original config here before it's resolved to functions
+    sourced = get_sourced_components(config)
+    nlp = load_model_from_config(raw_config, auto_fill=True)
+    logger.info("Set up nlp object from config")
+    config = nlp.config.interpolate()
+    # Resolve all training-relevant sections using the filled nlp config
+    T = registry.resolve(config["training"], schema=ConfigSchemaTraining)
+    D = registry.resolve(config["distillation"], schema=ConfigSchemaDistill)
+    dot_names = [T["dev_corpus"]]
+    if not isinstance(D["corpus"], str):
+        raise ConfigValidationError(
+            desc=Errors.E897.format(field="distillation.corpus", type=type(D["corpus"]))
+        )
+    if not isinstance(T["dev_corpus"], str):
+        raise ConfigValidationError(
+            desc=Errors.E897.format(
+                field="training.dev_corpus", type=type(T["dev_corpus"])
+            )
+        )
+    (dev_corpus,) = resolve_dot_names(config, dot_names)
+    optimizer = T["optimizer"]
+    # Components that shouldn't be updated during training
+    frozen_components = T["frozen_components"]
+    # Sourced components that require resume_training
+    resume_components = [p for p in sourced if p not in frozen_components]
     logger.info(f"Pipeline: {nlp.pipe_names}")
     if resume_components:
         with nlp.select_pipes(enable=resume_components):
             logger.info(f"Resuming training for: {resume_components}")
             nlp.resume_training(sgd=optimizer)
     # Make sure that listeners are defined before initializing further
     nlp._link_components()
+
+    # Get teacher labels to initialize student with.
+    student_to_teacher = D["student_to_teacher"]
+    teacher_pipes = dict(teacher.pipeline)
+    labels = {}
+    for name, pipe in nlp.pipeline:
+        # Copy teacher labels.
+        teacher_pipe_name = (
+            student_to_teacher[name] if name in student_to_teacher else name
+        )
+        teacher_pipe = teacher_pipes.get(teacher_pipe_name, None)
+        if (
+            teacher_pipe is not None
+            and getattr(teacher_pipe, "label_data", None) is not None
+        ):
+            labels[name] = teacher_pipe.label_data  # type: ignore[attr-defined]
+
     with nlp.select_pipes(disable=[*frozen_components, *resume_components]):
+        # Initialize on the dev corpus, since the distillation corpus does
+        # usually not have labels. Since we copy the labels from the teacher
+        # pipe, the dev data does not have to be exhaustive.
         if T["max_epochs"] == -1:
             sample_size = 100
             logger.debug(
                 f"Due to streamed train corpus, using only first {sample_size} "
                 f"examples for initialization. If necessary, provide all labels "
                 f"in [initialize]. More info: https://spacy.io/api/cli#init_labels"
             )
-            nlp.initialize(
-                lambda: islice(train_corpus(nlp), sample_size), sgd=optimizer
-            )
+            nlp.initialize(lambda: islice(dev_corpus(nlp), sample_size), sgd=optimizer)
         else:
-            nlp.initialize(lambda: train_corpus(nlp), sgd=optimizer)
+            nlp.initialize(lambda: dev_corpus(nlp), sgd=optimizer, labels=labels)
         logger.info(f"Initialized pipeline components: {nlp.pipe_names}")
     # Detect components with listeners that are not frozen consistently
     for name, proc in nlp.pipeline:
         for listener in getattr(
             proc, "listening_components", []
         ):  # e.g. tok2vec/transformer
             # Don't warn about components not in the pipeline
@@ -105,15 +195,15 @@
     *,
     data: Optional[Path] = None,
     lookups: Optional[Lookups] = None,
     vectors: Optional[str] = None,
 ) -> None:
     if lookups:
         nlp.vocab.lookups = lookups
-        logger.info(f"Added vocab lookups: {', '.join(lookups.tables)}")
+        logger.info("Added vocab lookups: %s", ", ".join(lookups.tables))
     data_path = ensure_path(data)
     if data_path is not None:
         lex_attrs = srsly.read_jsonl(data_path)
         for lexeme in nlp.vocab:
             lexeme.rank = OOV_RANK
         for attrs in lex_attrs:
             if "settings" in attrs:
@@ -121,25 +211,26 @@
             lexeme = nlp.vocab[attrs["orth"]]
             lexeme.set_attrs(**attrs)
         if len(nlp.vocab):
             oov_prob = min(lex.prob for lex in nlp.vocab) - 1
         else:
             oov_prob = DEFAULT_OOV_PROB
         nlp.vocab.cfg.update({"oov_prob": oov_prob})
-        logger.info(f"Added {len(nlp.vocab)} lexical entries to the vocab")
+        logger.info("Added %d lexical entries to the vocab", len(nlp.vocab))
     logger.info("Created vocabulary")
     if vectors is not None:
         load_vectors_into_model(nlp, vectors)
-        logger.info(f"Added vectors: {vectors}")
+        logger.info("Added vectors: %s", vectors)
     # warn if source model vectors are not identical
     sourced_vectors_hashes = nlp.meta.pop("_sourced_vectors_hashes", {})
-    vectors_hash = hash(nlp.vocab.vectors.to_bytes(exclude=["strings"]))
-    for sourced_component, sourced_vectors_hash in sourced_vectors_hashes.items():
-        if vectors_hash != sourced_vectors_hash:
-            warnings.warn(Warnings.W113.format(name=sourced_component))
+    if len(sourced_vectors_hashes) > 0:
+        vectors_hash = hash(nlp.vocab.vectors.to_bytes(exclude=["strings"]))
+        for sourced_component, sourced_vectors_hash in sourced_vectors_hashes.items():
+            if vectors_hash != sourced_vectors_hash:
+                warnings.warn(Warnings.W113.format(name=sourced_component))
     logger.info("Finished initializing nlp object")
 
 
 def load_vectors_into_model(
     nlp: "Language", name: Union[str, Path], *, add_strings: bool = True
 ) -> None:
     """Load word vectors from an installed model or path into a model instance."""
@@ -187,46 +278,45 @@
             errors = [{"loc": ["initialize", "init_tok2vec"], "msg": err}]
             raise ConfigValidationError(config=nlp.config, errors=errors)
         with init_tok2vec.open("rb") as file_:
             weights_data = file_.read()
     if weights_data is not None:
         layer = get_tok2vec_ref(nlp, P)
         layer.from_bytes(weights_data)
-        logger.info(f"Loaded pretrained weights from {init_tok2vec}")
+        logger.info("Loaded pretrained weights from %s", init_tok2vec)
         return True
     return False
 
 
 def convert_vectors(
     nlp: "Language",
     vectors_loc: Optional[Path],
     *,
     truncate: int,
     prune: int,
-    name: Optional[str] = None,
     mode: str = VectorsMode.default,
 ) -> None:
     vectors_loc = ensure_path(vectors_loc)
     if vectors_loc and vectors_loc.parts[-1].endswith(".npz"):
         nlp.vocab.vectors = Vectors(
             strings=nlp.vocab.strings, data=numpy.load(vectors_loc.open("rb"))
         )
         for lex in nlp.vocab:
             if lex.rank and lex.rank != OOV_RANK:
                 nlp.vocab.vectors.add(lex.orth, row=lex.rank)  # type: ignore[attr-defined]
         nlp.vocab.deduplicate_vectors()
     else:
         if vectors_loc:
-            logger.info(f"Reading vectors from {vectors_loc}")
+            logger.info("Reading vectors from %s", vectors_loc)
             vectors_data, vector_keys, floret_settings = read_vectors(
                 vectors_loc,
                 truncate,
                 mode=mode,
             )
-            logger.info(f"Loaded vectors from {vectors_loc}")
+            logger.info("Loaded vectors from %s", vectors_loc)
         else:
             vectors_data, vector_keys = (None, None)
         if vector_keys is not None and mode != VectorsMode.floret:
             for word in vector_keys:
                 if word not in nlp.vocab:
                     nlp.vocab[word]
         if vectors_data is not None:
@@ -237,20 +327,14 @@
                     **floret_settings,
                 )
             else:
                 nlp.vocab.vectors = Vectors(
                     strings=nlp.vocab.strings, data=vectors_data, keys=vector_keys
                 )
                 nlp.vocab.deduplicate_vectors()
-    if name is None:
-        # TODO: Is this correct? Does this matter?
-        nlp.vocab.vectors.name = f"{nlp.meta['lang']}_{nlp.meta['name']}.vectors"
-    else:
-        nlp.vocab.vectors.name = name
-    nlp.meta["vectors"]["name"] = nlp.vocab.vectors.name
     if prune >= 1 and mode != VectorsMode.floret:
         nlp.vocab.prune_vectors(prune)
 
 
 def read_vectors(
     vectors_loc: Path, truncate_vectors: int, *, mode: str = VectorsMode.default
 ):
```

### Comparing `spacy-4.0.0.dev0/spacy/training/iob_utils.py` & `spacy-4.0.0.dev1/spacy/training/iob_utils.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/loggers.py` & `spacy-4.0.0.dev1/spacy/training/loggers.py`

 * *Files identical despite different names*

### Comparing `spacy-4.0.0.dev0/spacy/training/pretrain.py` & `spacy-4.0.0.dev1/spacy/training/pretrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 def pretrain(
     config: Config,
     output_dir: Path,
     resume_path: Optional[Path] = None,
     epoch_resume: Optional[int] = None,
     use_gpu: int = -1,
     silent: bool = True,
+    skip_last: bool = False,
 ):
     msg = Printer(no_print=silent)
     if config["training"]["seed"] is not None:
         fix_random_seed(config["training"]["seed"])
     allocator = config["training"]["gpu_allocator"]
     if use_gpu >= 0 and allocator:
         set_gpu_allocator(allocator)
@@ -56,46 +57,54 @@
             f"Pre-training tok2vec layer - starting at epoch {epoch_resume} - saving every {P['n_save_epoch']} epoch"
         )
     else:
         msg.divider(f"Pre-training tok2vec layer - starting at epoch {epoch_resume}")
     row_settings = {"widths": (3, 10, 10, 6, 4), "aligns": ("r", "r", "r", "r", "r")}
     msg.row(("#", "# Words", "Total Loss", "Loss", "w/s"), **row_settings)
 
-    def _save_model(epoch, is_temp=False):
+    def _save_model(epoch, is_temp=False, is_last=False):
         is_temp_str = ".temp" if is_temp else ""
         with model.use_params(optimizer.averages):
-            with (output_dir / f"model{epoch}{is_temp_str}.bin").open("wb") as file_:
+            if is_last:
+                save_path = output_dir / f"model-last.bin"
+            else:
+                save_path = output_dir / f"model{epoch}{is_temp_str}.bin"
+            with (save_path).open("wb") as file_:
                 file_.write(model.get_ref("tok2vec").to_bytes())
             log = {
                 "nr_word": tracker.nr_word,
                 "loss": tracker.loss,
                 "epoch_loss": tracker.epoch_loss,
                 "epoch": epoch,
             }
             with (output_dir / "log.jsonl").open("a") as file_:
                 file_.write(srsly.json_dumps(log) + "\n")
 
     # TODO: I think we probably want this to look more like the
     # 'create_train_batches' function?
-    for epoch in range(epoch_resume, P["max_epochs"]):
-        for batch_id, batch in enumerate(batcher(corpus(nlp))):
-            docs = ensure_docs(batch)
-            loss = make_update(model, docs, optimizer, objective)
-            progress = tracker.update(epoch, loss, docs)
-            if progress:
-                msg.row(progress, **row_settings)
-            if P["n_save_every"] and (batch_id % P["n_save_every"] == 0):
-                _save_model(epoch, is_temp=True)
-
-        if P["n_save_epoch"]:
-            if epoch % P["n_save_epoch"] == 0 or epoch == P["max_epochs"] - 1:
+    try:
+        for epoch in range(epoch_resume, P["max_epochs"]):
+            for batch_id, batch in enumerate(batcher(corpus(nlp))):
+                docs = ensure_docs(batch)
+                loss = make_update(model, docs, optimizer, objective)
+                progress = tracker.update(epoch, loss, docs)
+                if progress:
+                    msg.row(progress, **row_settings)
+                if P["n_save_every"] and (batch_id % P["n_save_every"] == 0):
+                    _save_model(epoch, is_temp=True)
+
+            if P["n_save_epoch"]:
+                if epoch % P["n_save_epoch"] == 0 or epoch == P["max_epochs"] - 1:
+                    _save_model(epoch)
+            else:
                 _save_model(epoch)
-        else:
-            _save_model(epoch)
-        tracker.epoch_loss = 0.0
+            tracker.epoch_loss = 0.0
+    finally:
+        if not skip_last:
+            _save_model(P["max_epochs"], is_last=True)
 
 
 def ensure_docs(examples_or_docs: Iterable[Union[Doc, Example]]) -> List[Doc]:
     docs = []
     for eg_or_doc in examples_or_docs:
         if isinstance(eg_or_doc, Doc):
             docs.append(eg_or_doc)
```

### Comparing `spacy-4.0.0.dev0/spacy/ty.py` & `spacy-4.0.0.dev1/spacy/ty.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Protocol, runtime_checkable
 from typing import Optional, Any, Iterable, Dict, Callable, Sequence, List
-from .compat import Protocol, runtime_checkable
 
 from thinc.api import Optimizer, Model
 
 if TYPE_CHECKING:
     from .training import Example
+    from .language import Language
 
 
 @runtime_checkable
 class TrainableComponent(Protocol):
     model: Any
     is_trainable: bool
 
@@ -24,19 +24,38 @@
         ...
 
     def finish_update(self, sgd: Optimizer) -> None:
         ...
 
 
 @runtime_checkable
+class DistillableComponent(Protocol):
+    is_distillable: bool
+
+    def distill(
+        self,
+        teacher_pipe: Optional[TrainableComponent],
+        examples: Iterable["Example"],
+        *,
+        drop: float = 0.0,
+        sgd: Optional[Optimizer] = None,
+        losses: Optional[Dict[str, float]] = None
+    ) -> Dict[str, float]:
+        ...
+
+    def finish_update(self, sgd: Optimizer) -> None:
+        ...
+
+
+@runtime_checkable
 class InitializableComponent(Protocol):
     def initialize(
         self,
         get_examples: Callable[[], Iterable["Example"]],
-        nlp: Iterable["Example"],
+        nlp: "Language",
         **kwargs: Any
     ):
         ...
 
 
 @runtime_checkable
 class ListenedToComponent(Protocol):
```

### Comparing `spacy-4.0.0.dev0/spacy/util.py` & `spacy-4.0.0.dev1/spacy/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import List, Mapping, NoReturn, Union, Dict, Any, Set, cast
 from typing import Optional, Iterable, Callable, Tuple, Type
 from typing import Iterator, Pattern, Generator, TYPE_CHECKING
 from types import ModuleType
 import os
 import importlib
+import importlib.metadata
 import importlib.util
 import re
 from pathlib import Path
 import thinc
 from thinc.api import NumpyOps, get_current_ops, Adam, Config, Optimizer
 from thinc.api import ConfigValidationError, Model, constant as constant_schedule
+from thinc.api import fix_random_seed, set_gpu_allocator
 import functools
 import itertools
 import numpy
 import srsly
 import catalogue
 from catalogue import RegistryError, Registry
 import langcodes
@@ -28,37 +30,38 @@
 import tempfile
 import shutil
 import shlex
 import inspect
 import pkgutil
 import logging
 import socket
+import stat
 
 try:
     import cupy.random
 except ImportError:
     cupy = None
 
 
 from .symbols import ORTH
-from .compat import cupy, CudaStream, is_windows, importlib_metadata
+from .compat import cupy, CudaStream, is_windows
 from .errors import Errors, Warnings
 from . import about
 
 if TYPE_CHECKING:
     # This lets us add type hints for mypy etc. without causing circular imports
     from .language import Language, PipeCallable  # noqa: F401
     from .tokens import Doc, Span  # noqa: F401
     from .vocab import Vocab  # noqa: F401
 
 
 # fmt: off
 OOV_RANK = numpy.iinfo(numpy.uint64).max
 DEFAULT_OOV_PROB = -20
-LEXEME_NORM_LANGS = ["cs", "da", "de", "el", "en", "id", "lb", "mk", "pt", "ru", "sr", "ta", "th"]
+LEXEME_NORM_LANGS = ["cs", "da", "de", "el", "en", "grc", "id", "lb", "mk", "pt", "ru", "sr", "ta", "th"]
 
 # Default order of sections in the config file. Not all sections needs to exist,
 # and additional sections are added at the end, in alphabetical order.
 CONFIG_SECTION_ORDER = ["paths", "variables", "system", "nlp", "components", "corpora", "training", "pretraining", "initialize"]
 # fmt: on
 
 logger = logging.getLogger("spacy")
@@ -134,16 +137,25 @@
                 Errors.E893.format(
                     name=func_name, reg_name=registry_name, available=available
                 )
             ) from None
         return func
 
     @classmethod
-    def find(cls, registry_name: str, func_name: str) -> Callable:
-        """Get info about a registered function from the registry."""
+    def find(
+        cls, registry_name: str, func_name: str
+    ) -> Dict[str, Optional[Union[str, int]]]:
+        """Find information about a registered function, including the
+        module and path to the file it's defined in, the line number and the
+        docstring, if available.
+
+        registry_name (str): Name of the catalogue registry.
+        func_name (str): Name of the registered function.
+        RETURNS (Dict[str, Optional[Union[str, int]]]): The function info.
+        """
         # We're overwriting this classmethod so we're able to provide more
         # specific error messages and implement a fallback to spacy-legacy.
         if not hasattr(cls, registry_name):
             names = ", ".join(cls.get_registry_names()) or "none"
             raise RegistryError(Errors.E892.format(name=registry_name, available=names))
         reg = getattr(cls, registry_name)
         try:
@@ -278,15 +290,15 @@
     'zh'
     >>> find_matching_language('zxx')
     None
     """
     import spacy.lang  # noqa: F401
 
     if lang == "xx":
-        return "xx"
+        return "mul"
 
     # Find out which language modules we have
     possible_languages = []
     for modinfo in pkgutil.iter_modules(spacy.lang.__path__):  # type: ignore[attr-defined]
         code = modinfo.name
         if code == "xx":
             # Temporarily make 'xx' into a valid language code
@@ -296,19 +308,15 @@
 
     # Distances from 1-9 allow near misses like Bosnian -> Croatian and
     # Norwegian -> Norwegian Bokmål. A distance of 10 would include several
     # more possibilities, like variants of Chinese like 'wuu', but text that
     # is labeled that way is probably trying to be distinct from 'zh' and
     # shouldn't automatically match.
     match = langcodes.closest_supported_match(lang, possible_languages, max_distance=9)
-    if match == "mul":
-        # Convert 'mul' back to spaCy's 'xx'
-        return "xx"
-    else:
-        return match
+    return match
 
 
 def get_lang_class(lang: str) -> Type["Language"]:
     """Import and load a Language class.
 
     lang (str): IETF language code, such as 'en'.
     RETURNS (Language): Language class.
@@ -702,16 +710,16 @@
     """Get the version of an installed package. Typically used to get model
     package versions.
 
     name (str): The name of the installed Python package.
     RETURNS (str / None): The version or None if package not installed.
     """
     try:
-        return importlib_metadata.version(name)  # type: ignore[attr-defined]
-    except importlib_metadata.PackageNotFoundError:  # type: ignore[attr-defined]
+        return importlib.metadata.version(name)  # type: ignore[attr-defined]
+    except importlib.metadata.PackageNotFoundError:  # type: ignore[attr-defined]
         return None
 
 
 def is_compatible_version(
     version: str, constraint: str, prereleases: bool = True
 ) -> Optional[bool]:
     """Check if a version (e.g. "2.0.0") is compatible given a version
@@ -891,15 +899,15 @@
 def is_package(name: str) -> bool:
     """Check if string maps to a package installed via pip.
 
     name (str): Name of package.
     RETURNS (bool): True if installed package, False if not.
     """
     try:
-        importlib_metadata.distribution(name)  # type: ignore[attr-defined]
+        importlib.metadata.distribution(name)  # type: ignore[attr-defined]
         return True
     except:  # noqa: E722
         return False
 
 
 def get_package_path(name: str) -> Path:
     """Get the path to an installed package.
@@ -1029,16 +1037,23 @@
     """Execute a block in a temporary directory and remove the directory and
     its contents at the end of the with block.
 
     YIELDS (Path): The path of the temp directory.
     """
     d = Path(tempfile.mkdtemp())
     yield d
+
+    # On Windows, git clones use read-only files, which cause permission errors
+    # when being deleted. This forcibly fixes permissions.
+    def force_remove(rmfunc, path, ex):
+        os.chmod(path, stat.S_IWRITE)
+        rmfunc(path)
+
     try:
-        shutil.rmtree(str(d))
+        shutil.rmtree(str(d), onerror=force_remove)
     except PermissionError as e:
         warnings.warn(Warnings.W091.format(dir=d, msg=e))
 
 
 def is_cwd(path: Union[Path, str]) -> bool:
     """Check whether a path is the current working directory.
 
@@ -1714,15 +1729,15 @@
 # See licenses/3rd_party_licenses.txt
 def packages_distributions() -> Dict[str, List[str]]:
     """Return a mapping of top-level packages to their distributions. We're
     inlining this helper from the importlib_metadata "backport" here, since
     it's not available in the builtin importlib.metadata.
     """
     pkg_to_dist = defaultdict(list)
-    for dist in importlib_metadata.distributions():
+    for dist in importlib.metadata.distributions():
         for pkg in (dist.read_text("top_level.txt") or "").split():
             pkg_to_dist[pkg].append(dist.metadata["Name"])
     return dict(pkg_to_dist)
 
 
 def all_equal(iterable):
     """Return True if all the elements are equal to each other
@@ -1772,7 +1787,26 @@
 
     if port == 65535 and _is_port_in_use(port, host):
         raise ValueError(Errors.E1049.format(host=host))
 
     # if we get here, the port changed
     warnings.warn(Warnings.W124.format(host=host, port=start, serve_port=port))
     return port
+
+
+def set_gpu_allocator_from_config(config: Config, use_gpu: int):
+    """Change the global GPU allocator based to the value in
+    the configuration."""
+    if "gpu_allocator" not in config["training"]:
+        raise ValueError(Errors.E1015.format(value="[training] gpu_allocator"))
+    allocator = config["training"]["gpu_allocator"]
+    if use_gpu >= 0 and allocator:
+        set_gpu_allocator(allocator)
+
+
+def set_seed_from_config(config: Config):
+    """Set the random number generator seed to the value in
+    the configuration."""
+    if "seed" not in config["training"]:
+        raise ValueError(Errors.E1015.format(value="[training] seed"))
+    if config["training"]["seed"] is not None:
+        fix_random_seed(config["training"]["seed"])
```

### Comparing `spacy-4.0.0.dev0/spacy/vectors.pyx` & `spacy-4.0.0.dev1/spacy/vectors.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -48,48 +48,45 @@
 
     In floret mode, the floret settings (minn, maxn, etc.) are used to
     calculate the vector from the rows corresponding to the key's ngrams.
 
     DOCS: https://spacy.io/api/vectors
     """
     cdef public object strings
-    cdef public object name
     cdef readonly object mode
     cdef public object data
     cdef public object key2row
     cdef cppset[int] _unset
     cdef readonly uint32_t minn
     cdef readonly uint32_t maxn
     cdef readonly uint32_t hash_count
     cdef readonly uint32_t hash_seed
     cdef readonly unicode bow
     cdef readonly unicode eow
 
-    def __init__(self, *, strings=None, shape=None, data=None, keys=None, name=None, mode=Mode.default, minn=0, maxn=0, hash_count=1, hash_seed=0, bow="<", eow=">"):
+    def __init__(self, *, strings=None, shape=None, data=None, keys=None, mode=Mode.default, minn=0, maxn=0, hash_count=1, hash_seed=0, bow="<", eow=">"):
         """Create a new vector store.
 
         strings (StringStore): The string store.
         shape (tuple): Size of the table, as (# entries, # columns)
         data (numpy.ndarray or cupy.ndarray): The vector data.
         keys (iterable): A sequence of keys, aligned with the data.
-        name (str): A name to identify the vectors table.
         mode (str): Vectors mode: "default" or "floret" (default: "default").
         minn (int): The floret char ngram minn (default: 0).
         maxn (int): The floret char ngram maxn (default: 0).
         hash_count (int): The floret hash count (1-4, default: 1).
         hash_seed (int): The floret hash seed (default: 0).
         bow (str): The floret BOW string (default: "<").
         eow (str): The floret EOW string (default: ">").
 
         DOCS: https://spacy.io/api/vectors#init
         """
         self.strings = strings
         if self.strings is None:
             self.strings = StringStore()
-        self.name = name
         if mode not in Mode.values():
             raise ValueError(
                 Errors.E202.format(
                     name="vectors",
                     mode=mode,
                     modes=str(Mode.values())
                 )
```

### Comparing `spacy-4.0.0.dev0/spacy/vocab.pxd` & `spacy-4.0.0.dev1/spacy/vocab.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     cdef public object _lookups
     cdef public object writing_system
     cdef public object get_noun_chunks
     cdef readonly int length
     cdef public object lex_attr_getters
     cdef public object cfg
 
-    cdef const LexemeC* get(self, Pool mem, str string) except NULL
-    cdef const LexemeC* get_by_orth(self, Pool mem, attr_t orth) except NULL
+    cdef const LexemeC* get(self, str string) except NULL
+    cdef const LexemeC* get_by_orth(self, attr_t orth) except NULL
     cdef const TokenC* make_fused_token(self, substrings) except NULL
 
-    cdef const LexemeC* _new_lexeme(self, Pool mem, str string) except NULL
+    cdef const LexemeC* _new_lexeme(self, str string) except NULL
     cdef int _add_lex_to_vocab(self, hash_t key, const LexemeC* lex) except -1
-    cdef const LexemeC* _new_lexeme(self, Pool mem, str string) except NULL
 
     cdef PreshMap _by_orth
```

### Comparing `spacy-4.0.0.dev0/spacy/vocab.pyi` & `spacy-4.0.0.dev1/spacy/vocab.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 from .lookups import Lookups
 from .morphology import Morphology
 from .tokens import Doc, Span
 from .vectors import Vectors
 from pathlib import Path
 
 def create_vocab(
-    lang: Optional[str], defaults: Any, vectors_name: Optional[str] = ...
+    lang: Optional[str],
+    defaults: Any,
 ) -> Vocab: ...
 
 class Vocab:
     cfg: Dict[str, Any]
     get_noun_chunks: Optional[Callable[[Union[Doc, Span]], Iterator[Span]]]
     lookups: Lookups
     morphology: Morphology
     strings: StringStore
     vectors: Vectors
     writing_system: Dict[str, Any]
     def __init__(
         self,
         lex_attr_getters: Optional[Dict[str, Callable[[str], Any]]] = ...,
-        strings: Optional[Union[List[str], StringStore]] = ...,
+        strings: Optional[StringStore] = ...,
         lookups: Optional[Lookups] = ...,
         oov_prob: float = ...,
-        vectors_name: Optional[str] = ...,
         writing_system: Dict[str, Any] = ...,
         get_noun_chunks: Optional[Callable[[Union[Doc, Span]], Iterator[Span]]] = ...,
     ) -> None: ...
     @property
     def lang(self) -> str: ...
     def __len__(self) -> int: ...
     def add_flag(
```

### Comparing `spacy-4.0.0.dev0/spacy/vocab.pyx` & `spacy-4.0.0.dev1/spacy/vocab.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .util import registry
 from .lookups import Lookups
 from . import util
 from .lang.norm_exceptions import BASE_NORMS
 from .lang.lex_attrs import LEX_ATTRS, is_stop, get_lang
 
 
-def create_vocab(lang, defaults, vectors_name=None):
+def create_vocab(lang, defaults):
     # If the spacy-lookups-data package is installed, we pre-populate the lookups
     # with lexeme data, if available
     lex_attrs = {**LEX_ATTRS, **defaults.lex_attr_getters}
     # This is messy, but it's the minimal working fix to Issue #639.
     lex_attrs[IS_STOP] = functools.partial(is_stop, stops=defaults.stop_words)
     # Ensure that getter can be pickled
     lex_attrs[LANG] = functools.partial(get_lang, lang=lang)
@@ -35,56 +35,56 @@
         lex_attrs.get(NORM, LEX_ATTRS[NORM]),
         BASE_NORMS,
     )
     return Vocab(
         lex_attr_getters=lex_attrs,
         writing_system=defaults.writing_system,
         get_noun_chunks=defaults.syntax_iterators.get("noun_chunks"),
-        vectors_name=vectors_name,
     )
 
 
 cdef class Vocab:
     """A look-up table that allows you to access `Lexeme` objects. The `Vocab`
     instance also provides access to the `StringStore`, and owns underlying
     C-data that is shared between `Doc` objects.
 
     DOCS: https://spacy.io/api/vocab
     """
-    def __init__(self, lex_attr_getters=None, strings=tuple(), lookups=None,
-                 oov_prob=-20., vectors_name=None, writing_system={},
-                 get_noun_chunks=None, **deprecated_kwargs):
+    def __init__(self, lex_attr_getters=None, strings=None, lookups=None,
+            oov_prob=-20., writing_system=None, get_noun_chunks=None):
         """Create the vocabulary.
 
         lex_attr_getters (dict): A dictionary mapping attribute IDs to
             functions to compute them. Defaults to `None`.
         strings (StringStore): StringStore that maps strings to integers, and
             vice versa.
         lookups (Lookups): Container for large lookup tables and dictionaries.
         oov_prob (float): Default OOV probability.
-        vectors_name (str): Optional name to identify the vectors table.
         get_noun_chunks (Optional[Callable[[Union[Doc, Span], Iterator[Tuple[int, int, int]]]]]):
             A function that yields base noun phrases used for Doc.noun_chunks.
         """
         lex_attr_getters = lex_attr_getters if lex_attr_getters is not None else {}
         if lookups in (None, True, False):
             lookups = Lookups()
         self.cfg = {'oov_prob': oov_prob}
         self.mem = Pool()
         self._by_orth = PreshMap()
-        self.strings = StringStore()
         self.length = 0
-        if strings:
-            for string in strings:
-                _ = self[string]
+        if strings is None:
+            self.strings = StringStore()
+        else:
+            self.strings = strings
         self.lex_attr_getters = lex_attr_getters
         self.morphology = Morphology(self.strings)
-        self.vectors = Vectors(strings=self.strings, name=vectors_name)
+        self.vectors = Vectors(strings=self.strings)
         self.lookups = lookups
-        self.writing_system = writing_system
+        if writing_system is None:
+            self.writing_system = {}
+        else:
+            self.writing_system = writing_system
         self.get_noun_chunks = get_noun_chunks
 
     property vectors:
         def __get__(self):
             return self._vectors
 
         def __set__(self, vectors):
@@ -135,15 +135,15 @@
         elif flag_id >= 64 or flag_id < 1:
             raise ValueError(Errors.E063.format(value=flag_id))
         for lex in self:
             lex.set_flag(flag_id, flag_getter(lex.orth_))
         self.lex_attr_getters[flag_id] = flag_getter
         return flag_id
 
-    cdef const LexemeC* get(self, Pool mem, str string) except NULL:
+    cdef const LexemeC* get(self, str string) except NULL:
         """Get a pointer to a `LexemeC` from the lexicon, creating a new
         `Lexeme` if necessary using memory acquired from the given pool. If the
         pool is the lexicon's own memory, the lexeme is saved in the lexicon.
         """
         if string == "":
             return &EMPTY_LEXEME
         cdef LexemeC* lex
@@ -153,58 +153,46 @@
         if lex != NULL:
             assert lex.orth in self.strings
             if lex.orth != key:
                 raise KeyError(Errors.E064.format(string=lex.orth,
                                                   orth=key, orth_id=string))
             return lex
         else:
-            return self._new_lexeme(mem, string)
+            return self._new_lexeme(string)
 
-    cdef const LexemeC* get_by_orth(self, Pool mem, attr_t orth) except NULL:
+    cdef const LexemeC* get_by_orth(self, attr_t orth) except NULL:
         """Get a pointer to a `LexemeC` from the lexicon, creating a new
         `Lexeme` if necessary using memory acquired from the given pool. If the
         pool is the lexicon's own memory, the lexeme is saved in the lexicon.
         """
         if orth == 0:
             return &EMPTY_LEXEME
         cdef LexemeC* lex
         lex = <LexemeC*>self._by_orth.get(orth)
         if lex != NULL:
             return lex
         else:
-            return self._new_lexeme(mem, self.strings[orth])
+            return self._new_lexeme(self.strings[orth])
 
-    cdef const LexemeC* _new_lexeme(self, Pool mem, str string) except NULL:
-        # I think this heuristic is bad, and the Vocab should always
-        # own the lexemes. It avoids weird bugs this way, as it's how the thing
-        # was originally supposed to work. The best solution to the growing
-        # memory use is to periodically reset the vocab, which is an action
-        # that should be up to the user to do (so we don't need to keep track
-        # of the doc ownership).
-        # TODO: Change the C API so that the mem isn't passed in here.
-        mem = self.mem
-        #if len(string) < 3 or self.length < 10000:
-        #    mem = self.mem
-        cdef bint is_oov = mem is not self.mem
-        lex = <LexemeC*>mem.alloc(1, sizeof(LexemeC))
+    cdef const LexemeC* _new_lexeme(self, str string) except NULL:
+        lex = <LexemeC*>self.mem.alloc(1, sizeof(LexemeC))
         lex.orth = self.strings.add(string)
         lex.length = len(string)
         if self.vectors is not None:
             lex.id = self.vectors.key2row.get(lex.orth, OOV_RANK)
         else:
             lex.id = OOV_RANK
         if self.lex_attr_getters is not None:
             for attr, func in self.lex_attr_getters.items():
                 value = func(string)
                 if isinstance(value, str):
                     value = self.strings.add(value)
                 if value is not None:
                     Lexeme.set_struct_attr(lex, attr, value)
-        if not is_oov:
-            self._add_lex_to_vocab(lex.orth, lex)
+        self._add_lex_to_vocab(lex.orth, lex)
         if lex == NULL:
             raise ValueError(Errors.E085.format(string=string))
         return lex
 
     cdef int _add_lex_to_vocab(self, hash_t key, const LexemeC* lex) except -1:
         self._by_orth.set(lex.orth, <void*>lex)
         self.length += 1
@@ -267,15 +255,15 @@
     cdef const TokenC* make_fused_token(self, substrings) except NULL:
         cdef int i
         tokens = <TokenC*>self.mem.alloc(len(substrings) + 1, sizeof(TokenC))
         for i, props in enumerate(substrings):
             props = intify_attrs(props, strings_map=self.strings)
             token = &tokens[i]
             # Set the special tokens up to have arbitrary attributes
-            lex = <LexemeC*>self.get_by_orth(self.mem, props[ORTH])
+            lex = <LexemeC*>self.get_by_orth(props[ORTH])
             token.lex = lex
             for attr_id, value in props.items():
                 Token.set_struct_attr(token, attr_id, value)
                 # NORM is the only one that overlaps between the two
                 # (which is maybe not great?)
                 if attr_id != NORM:
                     Lexeme.set_struct_attr(lex, attr_id, value)
@@ -316,15 +304,15 @@
             return
         row_by_bytes = {row.tobytes(): i for i, row in enumerate(data)}
         key2row = {
             key: row_by_bytes[self.vectors.data[row].tobytes()]
             for key, row in self.vectors.key2row.items()
         }
         # replace vectors with deduplicated version
-        self.vectors = Vectors(strings=self.strings, data=data, name=self.vectors.name)
+        self.vectors = Vectors(strings=self.strings, data=data)
         for key, row in key2row.items():
             self.vectors.add(key, row=row)
 
     def prune_vectors(self, nr_row, batch_size=1024):
         """Reduce the current vector table to `nr_row` unique entries. Words
         mapped to the discarded vectors will be remapped to the closest vector
         among those remaining.
@@ -366,15 +354,15 @@
         priority = [(-lex.prob, self.vectors.key2row[lex.orth], lex.orth)
                     for lex in self if lex.orth in self.vectors.key2row]
         priority.sort()
         indices = xp.asarray([i for (prob, i, key) in priority], dtype="uint64")
         keys = xp.asarray([key for (prob, i, key) in priority], dtype="uint64")
         keep = xp.ascontiguousarray(self.vectors.data[indices[:nr_row]])
         toss = xp.ascontiguousarray(self.vectors.data[indices[nr_row:]])
-        self.vectors = Vectors(strings=self.strings, data=keep, keys=keys[:nr_row], name=self.vectors.name)
+        self.vectors = Vectors(strings=self.strings, data=keep, keys=keys[:nr_row])
         syn_keys, syn_rows, scores = self.vectors.most_similar(toss, batch_size=batch_size)
         syn_keys = ops.to_numpy(syn_keys)
         remap = {}
         for i, key in enumerate(ops.to_numpy(keys[nr_row:])):
             self.vectors.add(key, row=syn_rows[i][0])
             word = self.strings[key]
             synonym = self.strings[syn_keys[i][0]]
```

### Comparing `spacy-4.0.0.dev0/spacy.egg-info/PKG-INFO` & `spacy-4.0.0.dev1/spacy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy
-Version: 4.0.0.dev0
+Version: 4.0.0.dev1
 Summary: Industrial-strength Natural Language Processing (NLP) in Python
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spaCy/releases
 Project-URL: Source, https://github.com/explosion/spaCy
@@ -14,22 +14,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lookups
 Provides-Extra: transformers
 Provides-Extra: ray
 Provides-Extra: cuda
 Provides-Extra: cuda80
 Provides-Extra: cuda90
@@ -68,15 +66,18 @@
 state-of-the-art speed and **neural network models** for tagging,
 parsing, **named entity recognition**, **text classification** and more,
 multi-task learning with pretrained **transformers** like BERT, as well as a
 production-ready [**training system**](https://spacy.io/usage/training) and easy
 model packaging, deployment and workflow management. spaCy is commercial
 open-source software, released under the [MIT license](https://github.com/explosion/spaCy/blob/master/LICENSE).
 
-💫 **Version 3.4 out now!**
+💥 **We'd love to hear more about your experience with spaCy!**
+[Fill out our survey here.](https://form.typeform.com/to/aMel9q9f)
+
+💫 **Version 3.5 out now!**
 [Check out the release notes here.](https://github.com/explosion/spaCy/releases)
 
 [![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/8/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=8)
 [![Current Release Version](https://img.shields.io/github/release/explosion/spacy.svg?style=flat-square&logo=github)](https://github.com/explosion/spaCy/releases)
 [![pypi Version](https://img.shields.io/pypi/v/spacy.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy/)
 [![conda Version](https://img.shields.io/conda/vn/conda-forge/spacy.svg?style=flat-square&logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/spacy)
 [![Python wheels](https://img.shields.io/badge/wheels-%E2%9C%93-4c1.svg?longCache=true&style=flat-square&logo=python&logoColor=white)](https://github.com/explosion/wheelwright/releases)
@@ -84,43 +85,44 @@
 <br />
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/spacy?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/spacy/)
 [![Conda downloads](https://img.shields.io/conda/dn/conda-forge/spacy?label=conda%20downloads)](https://anaconda.org/conda-forge/spacy)
 [![spaCy on Twitter](https://img.shields.io/twitter/follow/spacy_io.svg?style=social&label=Follow)](https://twitter.com/spacy_io)
 
 ## 📖 Documentation
 
-| Documentation                                                                                                                                                                                                             |                                                                                                                                                                                                                                                                                                                              |
-| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| ⭐️ **[spaCy 101]**                                                                                                                                                                                                       | New to spaCy? Here's everything you need to know!                                                                                                                                                                                                                                                                            |
-| 📚 **[Usage Guides]**                                                                                                                                                                                                     | How to use spaCy and its features.                                                                                                                                                                                                                                                                                           |
-| 🚀 **[New in v3.0]**                                                                                                                                                                                                      | New features, backwards incompatibilities and migration guide.                                                                                                                                                                                                                                                               |
-| 🪐 **[Project Templates]**                                                                                                                                                                                                | End-to-end workflows you can clone, modify and run.                                                                                                                                                                                                                                                                          |
-| 🎛 **[API Reference]**                                                                                                                                                                                                     | The detailed reference for spaCy's API.                                                                                                                                                                                                                                                                                      |
-| 📦 **[Models]**                                                                                                                                                                                                           | Download trained pipelines for spaCy.                                                                                                                                                                                                                                                                                        |
-| 🌌 **[Universe]**                                                                                                                                                                                                         | Plugins, extensions, demos and books from the spaCy ecosystem.                                                                                                                                                                                                                                                               |
-| 👩‍🏫 **[Online Course]**                                                                                                                                                                                                    | Learn spaCy in this free and interactive online course.                                                                                                                                                                                                                                                                      |
-| 📺 **[Videos]**                                                                                                                                                                                                           | Our YouTube channel with video tutorials, talks and more.                                                                                                                                                                                                                                                                    |
-| 🛠 **[Changelog]**                                                                                                                                                                                                         | Changes and version history.                                                                                                                                                                                                                                                                                                 |
-| 💝 **[Contribute]**                                                                                                                                                                                                       | How to contribute to the spaCy project and code base.                                                                                                                                                                                                                                                                        |
+| Documentation                 |                                                                        |
+| ----------------------------- | ---------------------------------------------------------------------- |
+| ⭐️ **[spaCy 101]**           | New to spaCy? Here's everything you need to know!                      |
+| 📚 **[Usage Guides]**         | How to use spaCy and its features.                                     |
+| 🚀 **[New in v3.0]**          | New features, backwards incompatibilities and migration guide.         |
+| 🪐 **[Project Templates]**    | End-to-end workflows you can clone, modify and run.                    |
+| 🎛 **[API Reference]**         | The detailed reference for spaCy's API.                                |
+| 📦 **[Models]**               | Download trained pipelines for spaCy.                                  |
+| 🌌 **[Universe]**             | Plugins, extensions, demos and books from the spaCy ecosystem.         |
+| ⚙️ **[spaCy VS Code Extension]** | Additional tooling and features for working with spaCy's config files. |
+| 👩‍🏫 **[Online Course]** | Learn spaCy in this free and interactive online course. |
+| 📺 **[Videos]** | Our YouTube channel with video tutorials, talks and more. |
+| 🛠 **[Changelog]** | Changes and version history. |
+| 💝 **[Contribute]** | How to contribute to the spaCy project and code base. |
 | <a href="https://explosion.ai/spacy-tailored-pipelines"><img src="https://user-images.githubusercontent.com/13643239/152853098-1c761611-ccb0-4ec6-9066-b234552831fe.png" width="125" alt="spaCy Tailored Pipelines"/></a> | Get a custom spaCy pipeline, tailor-made for your NLP problem by spaCy's core developers. Streamlined, production-ready, predictable and maintainable. Start by completing our 5-minute questionnaire to tell us what you need and we'll be in touch! **[Learn more &rarr;](https://explosion.ai/spacy-tailored-pipelines)** |
 | <a href="https://explosion.ai/spacy-tailored-analysis"><img src="https://user-images.githubusercontent.com/1019791/206151300-b00cd189-e503-4797-aa1e-1bb6344062c5.png" width="125" alt="spaCy Tailored Pipelines"/></a> | Bespoke advice for problem solving, strategy and analysis for applied NLP projects. Services include data strategy, code reviews, pipeline design and annotation coaching. Curious? Fill in our 5-minute questionnaire to tell us what you need and we'll be in touch! **[Learn more &rarr;](https://explosion.ai/spacy-tailored-analysis)** |
 
 [spacy 101]: https://spacy.io/usage/spacy-101
 [new in v3.0]: https://spacy.io/usage/v3
 [usage guides]: https://spacy.io/usage/
 [api reference]: https://spacy.io/api/
 [models]: https://spacy.io/models
 [universe]: https://spacy.io/universe
+[spaCy VS Code Extension]: https://github.com/explosion/spacy-vscode
 [videos]: https://www.youtube.com/c/ExplosionAI
 [online course]: https://course.spacy.io
 [project templates]: https://github.com/explosion/projects
 [changelog]: https://spacy.io/usage#changelog
 [contribute]: https://github.com/explosion/spaCy/blob/master/CONTRIBUTING.md
 
-
 ## 💬 Where to ask questions
 
 The spaCy project is maintained by the [spaCy team](https://explosion.ai/about).
 Please understand that we won't be able to provide individual support via email.
 We also believe that help is much more valuable if it's shared publicly, so that
 more people can benefit from it.
 
@@ -157,15 +159,15 @@
 ## ⏳ Install spaCy
 
 For detailed installation instructions, see the
 [documentation](https://spacy.io/usage).
 
 - **Operating system**: macOS / OS X · Linux · Windows (Cygwin, MinGW, Visual
   Studio)
-- **Python version**: Python 3.6+ (only 64 bit)
+- **Python version**: Python 3.8+ (only 64 bit)
 - **Package managers**: [pip] · [conda] (via `conda-forge`)
 
 [pip]: https://pypi.org/project/spacy/
 [conda]: https://anaconda.org/conda-forge/spacy
 
 ### pip
```

#### html2text {}

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1 Name: spacy Version: 4.0.0.dev0 Summary: Industrial-
+Metadata-Version: 2.1 Name: spacy Version: 4.0.0.dev1 Summary: Industrial-
 strength Natural Language Processing (NLP) in Python Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Project-URL: Release notes, https://github.com/explosion/spaCy/releases
 Project-URL: Source, https://github.com/explosion/spaCy Classifier: Development
 Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Cython Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering Requires-Python: >=3.6 Description-
-Content-Type: text/markdown Provides-Extra: lookups Provides-Extra:
-transformers Provides-Extra: ray Provides-Extra: cuda Provides-Extra: cuda80
-Provides-Extra: cuda90 Provides-Extra: cuda91 Provides-Extra: cuda92 Provides-
-Extra: cuda100 Provides-Extra: cuda101 Provides-Extra: cuda102 Provides-Extra:
-cuda110 Provides-Extra: cuda111 Provides-Extra: cuda112 Provides-Extra: cuda113
-Provides-Extra: cuda114 Provides-Extra: cuda115 Provides-Extra: cuda116
-Provides-Extra: cuda117 Provides-Extra: cuda11x Provides-Extra: cuda-autodetect
-Provides-Extra: apple Provides-Extra: ja Provides-Extra: ko Provides-Extra: th
-License-File: LICENSE [https://explosion.ai/assets/img/logo.svg] # spaCy:
-Industrial-strength NLP spaCy is a library for **advanced Natural Language
-Processing** in Python and Cython. It's built on the very latest research, and
-was designed from day one to be used in real products. spaCy comes with
-[pretrained pipelines](https://spacy.io/models) and currently supports
-tokenization and training for **70+ languages**. It features state-of-the-art
-speed and **neural network models** for tagging, parsing, **named entity
-recognition**, **text classification** and more, multi-task learning with
-pretrained **transformers** like BERT, as well as a production-ready
-[**training system**](https://spacy.io/usage/training) and easy model
-packaging, deployment and workflow management. spaCy is commercial open-source
-software, released under the [MIT license](https://github.com/explosion/spaCy/
-blob/master/LICENSE). ð« **Version 3.4 out now!** [Check out the release
-notes here.](https://github.com/explosion/spaCy/releases) [![Azure Pipelines]
-(https://img.shields.io/azure-devops/build/explosion-ai/public/8/
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: lookups Provides-Extra: transformers Provides-Extra:
+ray Provides-Extra: cuda Provides-Extra: cuda80 Provides-Extra: cuda90
+Provides-Extra: cuda91 Provides-Extra: cuda92 Provides-Extra: cuda100 Provides-
+Extra: cuda101 Provides-Extra: cuda102 Provides-Extra: cuda110 Provides-Extra:
+cuda111 Provides-Extra: cuda112 Provides-Extra: cuda113 Provides-Extra: cuda114
+Provides-Extra: cuda115 Provides-Extra: cuda116 Provides-Extra: cuda117
+Provides-Extra: cuda11x Provides-Extra: cuda-autodetect Provides-Extra: apple
+Provides-Extra: ja Provides-Extra: ko Provides-Extra: th License-File: LICENSE
+[https://explosion.ai/assets/img/logo.svg] # spaCy: Industrial-strength NLP
+spaCy is a library for **advanced Natural Language Processing** in Python and
+Cython. It's built on the very latest research, and was designed from day one
+to be used in real products. spaCy comes with [pretrained pipelines](https://
+spacy.io/models) and currently supports tokenization and training for **70+
+languages**. It features state-of-the-art speed and **neural network models**
+for tagging, parsing, **named entity recognition**, **text classification** and
+more, multi-task learning with pretrained **transformers** like BERT, as well
+as a production-ready [**training system**](https://spacy.io/usage/training)
+and easy model packaging, deployment and workflow management. spaCy is
+commercial open-source software, released under the [MIT license](https://
+github.com/explosion/spaCy/blob/master/LICENSE). ð¥ **We'd love to hear more
+about your experience with spaCy!** [Fill out our survey here.](https://
+form.typeform.com/to/aMel9q9f) ð« **Version 3.5 out now!** [Check out the
+release notes here.](https://github.com/explosion/spaCy/releases) [![Azure
+Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/8/
 master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://
 dev.azure.com/explosion-ai/public/_build?definitionId=8) [![Current Release
 Version](https://img.shields.io/github/release/explosion/spacy.svg?style=flat-
 square&logo=github)](https://github.com/explosion/spaCy/releases) [![pypi
 Version](https://img.shields.io/pypi/v/spacy.svg?style=flat-
 square&logo=pypi&logoColor=white)](https://pypi.org/project/spacy/) [![conda
 Version](https://img.shields.io/conda/vn/conda-forge/spacy.svg?style=flat-
@@ -52,76 +52,73 @@
 github.com/ambv/black)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/
 spacy?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)]
 (https://pypi.org/project/spacy/) [![Conda downloads](https://img.shields.io/
 conda/dn/conda-forge/spacy?label=conda%20downloads)](https://anaconda.org/
 conda-forge/spacy) [![spaCy on Twitter](https://img.shields.io/twitter/follow/
 spacy_io.svg?style=social&label=Follow)](https://twitter.com/spacy_io) ## ð
-Documentation | Documentation | | | -------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
----------------- | ------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
--------------------------------------------------------------------------------
-------------------- | | â­ï¸ **[spaCy 101]** | New to spaCy? Here's
-everything you need to know! | | ð **[Usage Guides]** | How to use spaCy and
-its features. | | ð **[New in v3.0]** | New features, backwards
-incompatibilities and migration guide. | | ðª **[Project Templates]** | End-
-to-end workflows you can clone, modify and run. | | ð **[API Reference]** |
-The detailed reference for spaCy's API. | | ð¦ **[Models]** | Download
-trained pipelines for spaCy. | | ð **[Universe]** | Plugins, extensions,
-demos and books from the spaCy ecosystem. | | ð©âð« **[Online Course]** |
-Learn spaCy in this free and interactive online course. | | ðº **[Videos]** |
-Our YouTube channel with video tutorials, talks and more. | | ð  **
-[Changelog]** | Changes and version history. | | ð **[Contribute]** | How to
-contribute to the spaCy project and code base. | | [spaCy_Tailored_Pipelines] |
-Get a custom spaCy pipeline, tailor-made for your NLP problem by spaCy's core
-developers. Streamlined, production-ready, predictable and maintainable. Start
-by completing our 5-minute questionnaire to tell us what you need and we'll be
-in touch! **[Learn more →](https://explosion.ai/spacy-tailored-pipelines)** | |
+Documentation | Documentation | | | ----------------------------- | -----------
+----------------------------------------------------------- | | â­ï¸ **[spaCy
+101]** | New to spaCy? Here's everything you need to know! | | ð **[Usage
+Guides]** | How to use spaCy and its features. | | ð **[New in v3.0]** | New
+features, backwards incompatibilities and migration guide. | | ðª **[Project
+Templates]** | End-to-end workflows you can clone, modify and run. | | ð **
+[API Reference]** | The detailed reference for spaCy's API. | | ð¦ **
+[Models]** | Download trained pipelines for spaCy. | | ð **[Universe]** |
+Plugins, extensions, demos and books from the spaCy ecosystem. | | âï¸ **
+[spaCy VS Code Extension]** | Additional tooling and features for working with
+spaCy's config files. | | ð©âð« **[Online Course]** | Learn spaCy in this
+free and interactive online course. | | ðº **[Videos]** | Our YouTube channel
+with video tutorials, talks and more. | | ð  **[Changelog]** | Changes and
+version history. | | ð **[Contribute]** | How to contribute to the spaCy
+project and code base. | | [spaCy_Tailored_Pipelines] | Get a custom spaCy
+pipeline, tailor-made for your NLP problem by spaCy's core developers.
+Streamlined, production-ready, predictable and maintainable. Start by
+completing our 5-minute questionnaire to tell us what you need and we'll be in
+touch! **[Learn more →](https://explosion.ai/spacy-tailored-pipelines)** | |
 [spaCy_Tailored_Pipelines] | Bespoke advice for problem solving, strategy and
 analysis for applied NLP projects. Services include data strategy, code
 reviews, pipeline design and annotation coaching. Curious? Fill in our 5-minute
 questionnaire to tell us what you need and we'll be in touch! **[Learn more →]
 (https://explosion.ai/spacy-tailored-analysis)** | [spacy 101]: https://
 spacy.io/usage/spacy-101 [new in v3.0]: https://spacy.io/usage/v3 [usage
 guides]: https://spacy.io/usage/ [api reference]: https://spacy.io/api/
-[models]: https://spacy.io/models [universe]: https://spacy.io/universe
-[videos]: https://www.youtube.com/c/ExplosionAI [online course]: https://
-course.spacy.io [project templates]: https://github.com/explosion/projects
-[changelog]: https://spacy.io/usage#changelog [contribute]: https://github.com/
-explosion/spaCy/blob/master/CONTRIBUTING.md ## ð¬ Where to ask questions The
-spaCy project is maintained by the [spaCy team](https://explosion.ai/about).
-Please understand that we won't be able to provide individual support via
-email. We also believe that help is much more valuable if it's shared publicly,
-so that more people can benefit from it. | Type | Platforms | | ---------------
----------------- | --------------------------------------- | | ð¨ **Bug
-Reports** | [GitHub Issue Tracker] | | ð **Feature Requests & Ideas** |
-[GitHub Discussions] | | ð©âð» **Usage Questions** | [GitHub Discussions]
-Â· [Stack Overflow] | | ð¯ **General Discussion** | [GitHub Discussions] |
-[github issue tracker]: https://github.com/explosion/spaCy/issues [github
-discussions]: https://github.com/explosion/spaCy/discussions [stack overflow]:
-https://stackoverflow.com/questions/tagged/spacy ## Features - Support for
-**70+ languages** - **Trained pipelines** for different languages and tasks -
-Multi-task learning with pretrained **transformers** like BERT - Support for
+[models]: https://spacy.io/models [universe]: https://spacy.io/universe [spaCy
+VS Code Extension]: https://github.com/explosion/spacy-vscode [videos]: https:/
+/www.youtube.com/c/ExplosionAI [online course]: https://course.spacy.io
+[project templates]: https://github.com/explosion/projects [changelog]: https:/
+/spacy.io/usage#changelog [contribute]: https://github.com/explosion/spaCy/
+blob/master/CONTRIBUTING.md ## ð¬ Where to ask questions The spaCy project is
+maintained by the [spaCy team](https://explosion.ai/about). Please understand
+that we won't be able to provide individual support via email. We also believe
+that help is much more valuable if it's shared publicly, so that more people
+can benefit from it. | Type | Platforms | | ------------------------------- | -
+-------------------------------------- | | ð¨ **Bug Reports** | [GitHub Issue
+Tracker] | | ð **Feature Requests & Ideas** | [GitHub Discussions] | |
+ð©âð» **Usage Questions** | [GitHub Discussions] Â· [Stack Overflow] | |
+ð¯ **General Discussion** | [GitHub Discussions] | [github issue tracker]:
+https://github.com/explosion/spaCy/issues [github discussions]: https://
+github.com/explosion/spaCy/discussions [stack overflow]: https://
+stackoverflow.com/questions/tagged/spacy ## Features - Support for **70+
+languages** - **Trained pipelines** for different languages and tasks - Multi-
+task learning with pretrained **transformers** like BERT - Support for
 pretrained **word vectors** and embeddings - State-of-the-art speed -
 Production-ready **training system** - Linguistically-motivated
 **tokenization** - Components for named **entity recognition**, part-of-speech-
 tagging, dependency parsing, sentence segmentation, **text classification**,
 lemmatization, morphological analysis, entity linking and more - Easily
 extensible with **custom components** and attributes - Support for custom
 models in **PyTorch**, **TensorFlow** and other frameworks - Built in
 **visualizers** for syntax and NER - Easy **model packaging**, deployment and
 workflow management - Robust, rigorously evaluated accuracy ð **For more
 details, see the [facts, figures and benchmarks](https://spacy.io/usage/facts-
 figures).** ## â³ Install spaCy For detailed installation instructions, see
 the [documentation](https://spacy.io/usage). - **Operating system**: macOS / OS
 X Â· Linux Â· Windows (Cygwin, MinGW, Visual Studio) - **Python version**:
-Python 3.6+ (only 64 bit) - **Package managers**: [pip] Â· [conda] (via `conda-
+Python 3.8+ (only 64 bit) - **Package managers**: [pip] Â· [conda] (via `conda-
 forge`) [pip]: https://pypi.org/project/spacy/ [conda]: https://anaconda.org/
 conda-forge/spacy ### pip Using pip, spaCy releases are available as source
 packages and binary wheels. Before you install spaCy and its dependencies, make
 sure that your `pip`, `setuptools` and `wheel` are up to date. ```bash pip
 install -U pip setuptools wheel pip install spacy ``` To install additional
 data tables for lemmatization and normalization you can run `pip install spacy
 [lookups]` or install [`spacy-lookups-data`](https://github.com/explosion/
```

### Comparing `spacy-4.0.0.dev0/spacy.egg-info/SOURCES.txt` & `spacy-4.0.0.dev1/spacy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 spacy/__init__.py
 spacy/__main__.py
 spacy/about.py
 spacy/attrs.pxd
 spacy/attrs.pyx
 spacy/compat.py
 spacy/default_config.cfg
+spacy/default_config_distillation.cfg
 spacy/default_config_pretraining.cfg
 spacy/errors.py
 spacy/git_info.py
 spacy/glossary.py
 spacy/language.py
 spacy/lexeme.pxd
 spacy/lexeme.pyi
@@ -53,14 +54,15 @@
 spacy.egg-info/not-zip-safe
 spacy.egg-info/requires.txt
 spacy.egg-info/top_level.txt
 spacy/cli/__init__.py
 spacy/cli/_util.py
 spacy/cli/apply.py
 spacy/cli/assemble.py
+spacy/cli/benchmark_speed.py
 spacy/cli/convert.py
 spacy/cli/debug_config.py
 spacy/cli/debug_data.py
 spacy/cli/debug_diff.py
 spacy/cli/debug_model.py
 spacy/cli/download.py
 spacy/cli/evaluate.py
@@ -256,16 +258,16 @@
 spacy/lang/id/_tokenizer_exceptions_list.py
 spacy/lang/id/examples.py
 spacy/lang/id/lex_attrs.py
 spacy/lang/id/punctuation.py
 spacy/lang/id/stop_words.py
 spacy/lang/id/syntax_iterators.py
 spacy/lang/id/tokenizer_exceptions.py
-spacy/lang/is/__init__.py
-spacy/lang/is/stop_words.py
+spacy/lang/isl/__init__.py
+spacy/lang/isl/stop_words.py
 spacy/lang/it/__init__.py
 spacy/lang/it/examples.py
 spacy/lang/it/lemmatizer.py
 spacy/lang/it/punctuation.py
 spacy/lang/it/stop_words.py
 spacy/lang/it/syntax_iterators.py
 spacy/lang/it/tokenizer_exceptions.py
@@ -288,16 +290,18 @@
 spacy/lang/ky/__init__.py
 spacy/lang/ky/examples.py
 spacy/lang/ky/lex_attrs.py
 spacy/lang/ky/punctuation.py
 spacy/lang/ky/stop_words.py
 spacy/lang/ky/tokenizer_exceptions.py
 spacy/lang/la/__init__.py
+spacy/lang/la/examples.py
 spacy/lang/la/lex_attrs.py
 spacy/lang/la/stop_words.py
+spacy/lang/la/syntax_iterators.py
 spacy/lang/la/tokenizer_exceptions.py
 spacy/lang/lb/__init__.py
 spacy/lang/lb/examples.py
 spacy/lang/lb/lex_attrs.py
 spacy/lang/lb/punctuation.py
 spacy/lang/lb/stop_words.py
 spacy/lang/lb/tokenizer_exceptions.py
@@ -326,14 +330,24 @@
 spacy/lang/mk/tokenizer_exceptions.py
 spacy/lang/ml/__init__.py
 spacy/lang/ml/examples.py
 spacy/lang/ml/lex_attrs.py
 spacy/lang/ml/stop_words.py
 spacy/lang/mr/__init__.py
 spacy/lang/mr/stop_words.py
+spacy/lang/ms/__init__.py
+spacy/lang/ms/_tokenizer_exceptions_list.py
+spacy/lang/ms/examples.py
+spacy/lang/ms/lex_attrs.py
+spacy/lang/ms/punctuation.py
+spacy/lang/ms/stop_words.py
+spacy/lang/ms/syntax_iterators.py
+spacy/lang/ms/tokenizer_exceptions.py
+spacy/lang/mul/__init__.py
+spacy/lang/mul/examples.py
 spacy/lang/nb/__init__.py
 spacy/lang/nb/examples.py
 spacy/lang/nb/punctuation.py
 spacy/lang/nb/stop_words.py
 spacy/lang/nb/syntax_iterators.py
 spacy/lang/nb/tokenizer_exceptions.py
 spacy/lang/ne/__init__.py
@@ -394,19 +408,21 @@
 spacy/lang/sq/__init__.py
 spacy/lang/sq/examples.py
 spacy/lang/sq/stop_words.py
 spacy/lang/sr/__init__.py
 spacy/lang/sr/examples.py
 spacy/lang/sr/lemma_lookup_licence.txt
 spacy/lang/sr/lex_attrs.py
+spacy/lang/sr/punctuation.py
 spacy/lang/sr/stop_words.py
 spacy/lang/sr/tokenizer_exceptions.py
 spacy/lang/sv/__init__.py
 spacy/lang/sv/examples.py
 spacy/lang/sv/lex_attrs.py
+spacy/lang/sv/punctuation.py
 spacy/lang/sv/stop_words.py
 spacy/lang/sv/syntax_iterators.py
 spacy/lang/sv/tokenizer_exceptions.py
 spacy/lang/ta/__init__.py
 spacy/lang/ta/examples.py
 spacy/lang/ta/lex_attrs.py
 spacy/lang/ta/stop_words.py
@@ -456,16 +472,14 @@
 spacy/lang/ur/lex_attrs.py
 spacy/lang/ur/punctuation.py
 spacy/lang/ur/stop_words.py
 spacy/lang/vi/__init__.py
 spacy/lang/vi/examples.py
 spacy/lang/vi/lex_attrs.py
 spacy/lang/vi/stop_words.py
-spacy/lang/xx/__init__.py
-spacy/lang/xx/examples.py
 spacy/lang/yo/__init__.py
 spacy/lang/yo/examples.py
 spacy/lang/yo/lex_attrs.py
 spacy/lang/yo/stop_words.py
 spacy/lang/zh/__init__.py
 spacy/lang/zh/examples.py
 spacy/lang/zh/lex_attrs.py
@@ -491,14 +505,15 @@
 spacy/ml/staticvectors.py
 spacy/ml/tb_framework.pxd
 spacy/ml/tb_framework.pyx
 spacy/ml/models/__init__.py
 spacy/ml/models/entity_linker.py
 spacy/ml/models/multi_task.py
 spacy/ml/models/parser.py
+spacy/ml/models/span_finder.py
 spacy/ml/models/spancat.py
 spacy/ml/models/tagger.py
 spacy/ml/models/textcat.py
 spacy/ml/models/tok2vec.py
 spacy/pipeline/__init__.py
 spacy/pipeline/attribute_ruler.py
 spacy/pipeline/dep_parser.py
@@ -510,14 +525,15 @@
 spacy/pipeline/morphologizer.pyx
 spacy/pipeline/ner.py
 spacy/pipeline/pipe.pxd
 spacy/pipeline/pipe.pyi
 spacy/pipeline/pipe.pyx
 spacy/pipeline/sentencizer.pyx
 spacy/pipeline/senter.pyx
+spacy/pipeline/span_finder.py
 spacy/pipeline/span_ruler.py
 spacy/pipeline/spancat.py
 spacy/pipeline/tagger.pyx
 spacy/pipeline/textcat.py
 spacy/pipeline/textcat_multilabel.py
 spacy/pipeline/tok2vec.py
 spacy/pipeline/trainable_pipe.pxd
@@ -546,16 +562,14 @@
 spacy/pipeline/_parser_internals/nonproj.pyx
 spacy/pipeline/_parser_internals/search.pxd
 spacy/pipeline/_parser_internals/search.pyx
 spacy/pipeline/_parser_internals/stateclass.pxd
 spacy/pipeline/_parser_internals/stateclass.pyx
 spacy/pipeline/_parser_internals/transition_system.pxd
 spacy/pipeline/_parser_internals/transition_system.pyx
-spacy/pipeline/legacy/__init__.py
-spacy/pipeline/legacy/entity_linker.py
 spacy/tests/__init__.py
 spacy/tests/conftest.py
 spacy/tests/enable_gpu.py
 spacy/tests/test_architectures.py
 spacy/tests/test_cli.py
 spacy/tests/test_cli_app.py
 spacy/tests/test_displacy.py
@@ -676,17 +690,17 @@
 spacy/tests/lang/hy/__init__.py
 spacy/tests/lang/hy/test_text.py
 spacy/tests/lang/hy/test_tokenizer.py
 spacy/tests/lang/id/__init__.py
 spacy/tests/lang/id/test_noun_chunks.py
 spacy/tests/lang/id/test_prefix_suffix_infix.py
 spacy/tests/lang/id/test_text.py
-spacy/tests/lang/is/__init__.py
-spacy/tests/lang/is/test_text.py
-spacy/tests/lang/is/test_tokenizer.py
+spacy/tests/lang/isl/__init__.py
+spacy/tests/lang/isl/test_text.py
+spacy/tests/lang/isl/test_tokenizer.py
 spacy/tests/lang/it/__init__.py
 spacy/tests/lang/it/test_noun_chunks.py
 spacy/tests/lang/it/test_prefix_suffix_infix.py
 spacy/tests/lang/it/test_stopwords.py
 spacy/tests/lang/it/test_text.py
 spacy/tests/lang/ja/__init__.py
 spacy/tests/lang/ja/test_lemmatization.py
@@ -697,14 +711,15 @@
 spacy/tests/lang/ko/test_lemmatization.py
 spacy/tests/lang/ko/test_serialize.py
 spacy/tests/lang/ko/test_tokenizer.py
 spacy/tests/lang/ky/__init__.py
 spacy/tests/lang/ky/test_tokenizer.py
 spacy/tests/lang/la/__init__.py
 spacy/tests/lang/la/test_exception.py
+spacy/tests/lang/la/test_noun_chunks.py
 spacy/tests/lang/la/test_text.py
 spacy/tests/lang/lb/__init__.py
 spacy/tests/lang/lb/test_exceptions.py
 spacy/tests/lang/lb/test_prefix_suffix_infix.py
 spacy/tests/lang/lb/test_text.py
 spacy/tests/lang/lg/__init__.py
 spacy/tests/lang/lg/test_tokenizer.py
@@ -713,14 +728,21 @@
 spacy/tests/lang/lv/__init__.py
 spacy/tests/lang/lv/test_text.py
 spacy/tests/lang/lv/test_tokenizer.py
 spacy/tests/lang/mk/__init__.py
 spacy/tests/lang/mk/test_text.py
 spacy/tests/lang/ml/__init__.py
 spacy/tests/lang/ml/test_text.py
+spacy/tests/lang/ms/__init__.py
+spacy/tests/lang/ms/test_noun_chunks.py
+spacy/tests/lang/ms/test_prefix_suffix_infix.py
+spacy/tests/lang/ms/test_text.py
+spacy/tests/lang/mul/__init__.py
+spacy/tests/lang/mul/test_text.py
+spacy/tests/lang/mul/test_tokenizer.py
 spacy/tests/lang/nb/__init__.py
 spacy/tests/lang/nb/test_noun_chunks.py
 spacy/tests/lang/nb/test_tokenizer.py
 spacy/tests/lang/ne/__init__.py
 spacy/tests/lang/ne/test_text.py
 spacy/tests/lang/nl/__init__.py
 spacy/tests/lang/nl/test_noun_chunks.py
@@ -785,17 +807,14 @@
 spacy/tests/lang/uk/test_tokenizer_exc.py
 spacy/tests/lang/ur/__init__.py
 spacy/tests/lang/ur/test_prefix_suffix_infix.py
 spacy/tests/lang/ur/test_text.py
 spacy/tests/lang/vi/__init__.py
 spacy/tests/lang/vi/test_serialize.py
 spacy/tests/lang/vi/test_tokenizer.py
-spacy/tests/lang/xx/__init__.py
-spacy/tests/lang/xx/test_text.py
-spacy/tests/lang/xx/test_tokenizer.py
 spacy/tests/lang/yo/__init__.py
 spacy/tests/lang/yo/test_text.py
 spacy/tests/lang/zh/__init__.py
 spacy/tests/lang/zh/test_serialize.py
 spacy/tests/lang/zh/test_text.py
 spacy/tests/lang/zh/test_tokenizer.py
 spacy/tests/matcher/__init__.py
@@ -814,14 +833,15 @@
 spacy/tests/package/requirements.txt
 spacy/tests/package/setup.cfg
 spacy/tests/package/test_requirements.py
 spacy/tests/parser/__init__.py
 spacy/tests/parser/_search.pyx
 spacy/tests/parser/test_add_label.py
 spacy/tests/parser/test_arc_eager_oracle.py
+spacy/tests/parser/test_model.py
 spacy/tests/parser/test_ner.py
 spacy/tests/parser/test_neural_parser.py
 spacy/tests/parser/test_nn_beam.py
 spacy/tests/parser/test_nonproj.py
 spacy/tests/parser/test_parse.py
 spacy/tests/parser/test_parse_navigate.py
 spacy/tests/parser/test_preset_sbd.py
@@ -840,14 +860,15 @@
 spacy/tests/pipeline/test_lemmatizer.py
 spacy/tests/pipeline/test_models.py
 spacy/tests/pipeline/test_morphologizer.py
 spacy/tests/pipeline/test_pipe_factories.py
 spacy/tests/pipeline/test_pipe_methods.py
 spacy/tests/pipeline/test_sentencizer.py
 spacy/tests/pipeline/test_senter.py
+spacy/tests/pipeline/test_span_finder.py
 spacy/tests/pipeline/test_span_ruler.py
 spacy/tests/pipeline/test_spancat.py
 spacy/tests/pipeline/test_tagger.py
 spacy/tests/pipeline/test_textcat.py
 spacy/tests/pipeline/test_tok2vec.py
 spacy/tests/serialize/__init__.py
 spacy/tests/serialize/test_resource_warning.py
@@ -867,15 +888,17 @@
 spacy/tests/tokenizer/test_explain.py
 spacy/tests/tokenizer/test_naughty_strings.py
 spacy/tests/tokenizer/test_tokenizer.py
 spacy/tests/tokenizer/test_urls.py
 spacy/tests/tokenizer/test_whitespace.py
 spacy/tests/training/__init__.py
 spacy/tests/training/test_augmenters.py
+spacy/tests/training/test_corpus.py
 spacy/tests/training/test_logger.py
+spacy/tests/training/test_loop.py
 spacy/tests/training/test_new_example.py
 spacy/tests/training/test_pretraining.py
 spacy/tests/training/test_readers.py
 spacy/tests/training/test_rehearse.py
 spacy/tests/training/test_training.py
 spacy/tests/vocab_vectors/__init__.py
 spacy/tests/vocab_vectors/test_lexeme.py
```

### Comparing `spacy-4.0.0.dev0/spacy.egg-info/requires.txt` & `spacy-4.0.0.dev1/spacy.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,84 @@
-spacy-legacy<3.1.0,>=3.0.11
+spacy-legacy<4.1.0,>=4.0.0.dev0
 spacy-loggers<2.0.0,>=1.0.0
 murmurhash<1.1.0,>=0.28.0
 cymem<2.1.0,>=2.0.2
 preshed<3.1.0,>=3.0.2
 thinc<9.1.0,>=9.0.0.dev2
 wasabi<1.2.0,>=0.9.1
 srsly<3.0.0,>=2.4.3
 catalogue<2.1.0,>=2.0.6
-typer<0.8.0,>=0.3.0
+typer<0.10.0,>=0.3.0
 pathy>=0.10.0
 smart-open<7.0.0,>=5.2.1
 tqdm<5.0.0,>=4.38.0
 numpy>=1.15.0
 requests<3.0.0,>=2.13.0
 pydantic!=1.8,!=1.8.1,<1.11.0,>=1.7.4
 jinja2
 setuptools
 packaging>=20.0
 langcodes<4.0.0,>=3.2.0
 
-[:python_version < "3.8"]
-typing_extensions<4.2.0,>=3.7.4
-
 [apple]
 thinc-apple-ops<1.0.0,>=0.1.0.dev0
 
 [cuda]
-cupy<12.0.0,>=5.0.0b4
+cupy<13.0.0,>=5.0.0b4
 
 [cuda-autodetect]
-cupy-wheel<12.0.0,>=11.0.0
+cupy-wheel<13.0.0,>=11.0.0
 
 [cuda100]
-cupy-cuda100<12.0.0,>=5.0.0b4
+cupy-cuda100<13.0.0,>=5.0.0b4
 
 [cuda101]
-cupy-cuda101<12.0.0,>=5.0.0b4
+cupy-cuda101<13.0.0,>=5.0.0b4
 
 [cuda102]
-cupy-cuda102<12.0.0,>=5.0.0b4
+cupy-cuda102<13.0.0,>=5.0.0b4
 
 [cuda110]
-cupy-cuda110<12.0.0,>=5.0.0b4
+cupy-cuda110<13.0.0,>=5.0.0b4
 
 [cuda111]
-cupy-cuda111<12.0.0,>=5.0.0b4
+cupy-cuda111<13.0.0,>=5.0.0b4
 
 [cuda112]
-cupy-cuda112<12.0.0,>=5.0.0b4
+cupy-cuda112<13.0.0,>=5.0.0b4
 
 [cuda113]
-cupy-cuda113<12.0.0,>=5.0.0b4
+cupy-cuda113<13.0.0,>=5.0.0b4
 
 [cuda114]
-cupy-cuda114<12.0.0,>=5.0.0b4
+cupy-cuda114<13.0.0,>=5.0.0b4
 
 [cuda115]
-cupy-cuda115<12.0.0,>=5.0.0b4
+cupy-cuda115<13.0.0,>=5.0.0b4
 
 [cuda116]
-cupy-cuda116<12.0.0,>=5.0.0b4
+cupy-cuda116<13.0.0,>=5.0.0b4
 
 [cuda117]
-cupy-cuda117<12.0.0,>=5.0.0b4
+cupy-cuda117<13.0.0,>=5.0.0b4
 
 [cuda11x]
-cupy-cuda11x<12.0.0,>=11.0.0
+cupy-cuda11x<13.0.0,>=11.0.0
 
 [cuda80]
-cupy-cuda80<12.0.0,>=5.0.0b4
+cupy-cuda80<13.0.0,>=5.0.0b4
 
 [cuda90]
-cupy-cuda90<12.0.0,>=5.0.0b4
+cupy-cuda90<13.0.0,>=5.0.0b4
 
 [cuda91]
-cupy-cuda91<12.0.0,>=5.0.0b4
+cupy-cuda91<13.0.0,>=5.0.0b4
 
 [cuda92]
-cupy-cuda92<12.0.0,>=5.0.0b4
+cupy-cuda92<13.0.0,>=5.0.0b4
 
 [ja]
 sudachipy!=0.6.1,>=0.5.2
 sudachidict_core>=20211220
 
 [ko]
 mecab-ko>=1.0.0
```

