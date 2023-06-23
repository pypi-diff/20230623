# Comparing `tmp/khoj_assistant-0.6.3.dev81.tar.gz` & `tmp/khoj_assistant-0.6.3.dev88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jun 21 19:34:53 2023, max compression
+gzip compressed data, last modified: Fri Jun 23 21:39:25 2023, max compression
```

## Comparing `khoj_assistant-0.6.3.dev81.tar` & `khoj_assistant-0.6.3.dev88.tar`

### file list

```diff
@@ -1,74 +1,80 @@
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/__init__.py
--rw-r--r--   0        0        0    10848 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/configure.py
--rw-r--r--   0        0        0     4929 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     1362 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      647 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/base_data_integration.html
--rw-r--r--   0        0        0      657 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0     9835 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     2151 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     3671 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     5756 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    12548 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     2872 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0   275822 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58507 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0   205167 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0    13011 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6053 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0     6985 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     6891 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     6533 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16789 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5160 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    13101 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     3866 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      463 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7470 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2713 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3690 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    10930 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2494 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/config.py
--rw-r--r--   0        0        0     3070 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6779 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4158 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1047 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/.gitignore
--rw-r--r--   0        0        0    32472 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/LICENSE
--rw-r--r--   0        0        0    22944 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/README.md
--rw-r--r--   0        0        0     2781 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/pyproject.toml
--rw-r--r--   0        0        0    25280 2023-06-21 19:34:53.000000 khoj_assistant-0.6.3.dev81/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/__init__.py
+-rw-r--r--   0        0        0    10848 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/configure.py
+-rw-r--r--   0        0        0     4929 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/file_browser.py
+-rw-r--r--   0        0        0      987 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/labelled_text_field.py
+-rw-r--r--   0        0        0    17819 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1316 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3290 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0     9894 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     5971 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     4394 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6565 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    12744 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3410 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1828 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58507 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6053 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0     6985 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     6891 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     6533 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16789 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5160 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    13101 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     3866 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      463 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7470 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2713 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3690 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    10930 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2012 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2494 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     3070 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6779 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4158 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1047 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/.gitignore
+-rw-r--r--   0        0        0    32472 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/LICENSE
+-rw-r--r--   0        0        0    22944 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/README.md
+-rw-r--r--   0        0        0     2781 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/pyproject.toml
+-rw-r--r--   0        0        0    25280 2023-06-23 21:39:25.000000 khoj_assistant-0.6.3.dev88/PKG-INFO
```

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/configure.py` & `khoj_assistant-0.6.3.dev88/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/main.py` & `khoj_assistant-0.6.3.dev88/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/file_browser.py` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/file_browser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/labelled_text_field.py` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/labelled_text_field.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/404.html` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/base_data_integration.html` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/base_processor_integration.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!DOCTYPE html>
 <html>
   	<head>
-    	<title>Khoj: Data Settings</title>
+    	<title>Khoj: Processor Settings</title>
     	<link rel=”stylesheet” href=”static/styles.css”>
     	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@picocss/pico@1/css/pico.min.css">
   	</head>
   	<body class="data-integration">
     	<header class=”header”>
-      	<h1>Configure your data integrations for Khoj</h1>
+      	<h1>Configure your processor integrations for Khoj</h1>
     	</header>
 		<a href="/config">Go back</a>
 
     	<div class=”content”>
       		{% block content %}
       		{% endblock %}
     	</div>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 
-****** Configure your data integrations for Khoj ******
+****** Configure your processor integrations for Khoj ******
  Go_back
 {% block content %} {% endblock %}
```

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/chat.html` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/chat.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1.0">
         <title>Khoj - Chat</title>
 
         <link rel="icon" type="image/png" sizes="128x128" href="/static/assets/icons/favicon-128x128.png">
         <link rel="manifest" href="/static/khoj_chat.webmanifest">
+        <link rel="stylesheet" href="/static/assets/khoj.css">
     </head>
     <script>
         function formatDate(date) {
             // Format date in HH:MM, DD MMM YYYY format
             let time_string = date.toLocaleTimeString('en-IN', { hour: '2-digit', minute: '2-digit', hour12: false });
             let date_string = date.toLocaleString('en-IN', { year: 'numeric', month: 'short', day: '2-digit'}).replaceAll('-', ' ');
             return `${time_string}, ${date_string}`;
@@ -99,33 +100,34 @@
             if (query_via_url) {
                 document.getElementById("chat-input").value = query_via_url;
                 chat();
             }
         }
     </script>
     <body>
-        <!-- Chat Header -->
-        <h1>
-            <img class="khoj-logo" src="static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
-        </h1>
+       <!--Add Header Logo and Nav Pane-->
+        <div class="khoj-header">
+            <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+            <nav class="khoj-nav">
+                <a class="khoj-nav-selected" href="/chat">Chat</a>
+                <a href="/">Search</a>
+                <a href="/config">Settings</a>
+            </nav>
+        </div>
 
         <!-- Chat Body -->
         <div id="chat-body"></div>
 
         <!-- Chat Footer -->
         <div id="chat-footer">
             <input type="text" id="chat-input" class="option" onkeyup=incrementalChat(event) autofocus="autofocus" placeholder="What is the meaning of life?">
         </div>
     </body>
 
     <style>
-        :root {
-            --night-black: #282c34;
-            --evening-sun: #fbb912;
-        }
         html, body {
             height: 100%;
             width: 100%;
             padding: 0px;
             margin: 0px;
         }
         body {
@@ -138,22 +140,14 @@
             font-weight: 300;
             line-height: 1.5em;
         }
         body > * {
             padding: 10px;
             margin: 10px;
         }
-        h1 {
-            margin: 8px 0;
-            padding: 0;
-        }
-        img.khoj-logo {
-            width: min(60vw, 150px);
-        }
-
         #chat-body {
             font-size: medium;
             margin: 0px;
             line-height: 20px;
             overflow-y: scroll; /* Make chat body scroll to see history */
         }
         /* add chat metatdata to bottom of bubble */
@@ -182,27 +176,27 @@
             position: relative;
             display: inline-block;
             max-width: 80%;
             text-align: left;
         }
         /* color chat bubble by khoj blue */
         .chat-message-text.khoj {
-            color: var(--night-black);
-            background: var(--evening-sun);
+            color: var(--primary-inverse);
+            background: var(--primary);
             margin-left: auto;
             white-space: pre-line;
         }
         /* add left protrusion to khoj chat bubble */
         .chat-message-text.khoj:after {
             content: '';
             position: absolute;
             bottom: -2px;
             left: -7px;
             border: 10px solid transparent;
-            border-top-color: var(--evening-sun);
+            border-top-color: var(--primary);
             border-bottom: 0;
             transform: rotate(-60deg);
         }
         /* color chat bubble by you dark grey */
         .chat-message-text.you {
             color: #f8fafc;
             background: #475569;
```

#### html2text {}

```diff
@@ -1,4 +1,5 @@
 
 
-****** [Khoj] ******
+
+[Khoj]  Chat Search Settings
 [                    ]
```

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/processor_conversation_input.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,78 @@
-{% extends "base_data_integration.html" %}
+{% extends "base_config.html" %}
 {% block content %}
-<h2>Github</h2>
-<form id="config-form">
-    <div id="success" style="display: none;"></div>
-    <table>
-        <tr>
-            <td>
-                <label for="pat-token">Personal Access Token</label>
-            </td>
-            <td>
-                <input type="text" id="pat-token" name="pat" value="{{ current_config['pat_token'] }}">
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="repo-owner">Repository Owner</label>
-            </td>
-            <td>
-                <input type="text" id="repo-owner" name="repo_owner" value="{{ current_config['repo_owner'] }}">
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="repo-name">Repository Name</label>
-            </td>
-            <td>
-                <input type="text" id="repo-name" name="repo_name" value="{{ current_config['repo_name'] }}">
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="repo-branch">Repository Branch</label>
-            </td>
-            <td>
-                <input type="text" id="repo-branch" name="repo_branch" value="{{ current_config['repo_branch'] }}">
-            </td>
-        </tr>
-    </table>
-    <h4>You probably don't need to edit these.</h4>
+<div class="page">
+    <div class="section">
+        <h2 class="section-title">
+            <img class="card-icon" src="/static/assets/icons/chat.svg" alt="Chat">
+            <span class="card-title-text">Chat</span>
+        </h2>
+        <form id="config-form">
+            <div id="success" style="display: none;" ></div>
+            <table>
+                <tr>
+                    <td>
+                        <label for="openai-api-key">OpenAI API key</label>
+                    </td>
+                    <td>
+                        <input type="text" id="openai-api-key" name="openai-api-key" value="{{ current_config['openai_api_key'] }}">
+                    </td>
+                </tr>
+            </table>
 
-    <table>
-        <tr>
-            <td>
-                <label for="compressed-jsonl">Compressed JSONL (Output)</label>
-            </td>
-            <td>
-                <input type="text" id="compressed-jsonl" name="compressed-jsonl" value="{{ current_config['compressed_jsonl'] }}">
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="embeddings-file">Embeddings File (Output)</label>
-            </td>
-            <td>
-                <input type="text" id="embeddings-file" name="embeddings-file" value="{{ current_config['embeddings_file'] }}">
-            </td>
-        </tr>
-    </table>
-    <button id="submit" type="submit">Submit</button>
-</form>
+            <h4>You probably don't need to edit these.</h4>
+
+            <table>
+                <tr>
+                    <td>
+                        <label for="conversation-logfile">Conversation Logfile</label>
+                    </td>
+                    <td>
+                        <input type="text" id="conversation-logfile" name="conversation-logfile" value="{{ current_config['conversation_logfile'] }}">
+                    </td>
+                </tr>
+                <tr>
+                    <td>
+                        <label for="model">Model</label>
+                    </td>
+                    <td>
+                        <input type="text" id="model" name="model" value="{{ current_config['model'] }}">
+                    </td>
+                </tr>
+                <tr>
+                    <td>
+                        <label for="chat-model">Chat Model</label>
+                    </td>
+                    <td>
+                        <input type="text" id="chat-model" name="chat-model" value="{{ current_config['chat_model'] }}">
+                    </td>
+                </tr>
+            </table>
+            <button id="submit" type="submit">Save</button>
+        </form>
+    </div>
+</div>
 <script>
     submit.addEventListener("click", function(event) {
         event.preventDefault();
+        var openai_api_key = document.getElementById("openai-api-key").value;
+        var conversation_logfile = document.getElementById("conversation-logfile").value;
+        var model = document.getElementById("model").value;
+        var chat_model = document.getElementById("chat-model").value;
 
-        var compressed_jsonl = document.getElementById("compressed-jsonl").value;
-        var embeddings_file = document.getElementById("embeddings-file").value;
-        var pat_token = document.getElementById("pat-token").value;
-        var repo_owner = document.getElementById("repo-owner").value;
-        var repo_name = document.getElementById("repo-name").value;
-        var repo_branch = document.getElementById("repo-branch").value;
-
-        fetch('/api/config/data/content_type/github', {
+        fetch('/api/config/data/processor/conversation', {
             method: 'POST',
             headers: {
                 'Content-Type': 'application/json',
             },
             body: JSON.stringify({
-                "pat_token": pat_token,
-                "repo_owner": repo_owner,
-                "repo_name": repo_name,
-                "repo_branch": repo_branch,
-                "compressed_jsonl": compressed_jsonl,
-                "embeddings_file": embeddings_file,
+                "openai_api_key": openai_api_key,
+                "conversation_logfile": conversation_logfile,
+                "model": model,
+                "chat_model": chat_model
             })
         })
         .then(response => response.json())
         .then(data => {
             if (data["status"] == "ok") {
                 document.getElementById("success").innerHTML = "✅ Successfully updated. Go to <a href='/config'>your settings</a> to regenerate your index.";
                 document.getElementById("success").style.display = "block";
```

#### html2text {}

```diff
@@ -1,11 +1,9 @@
-{% extends "base_data_integration.html" %} {% block content %}
-***** Github *****
-Personal Access Token [{{ current_config['pat_token'] }}]
-Repository Owner      [{{ current_config['repo_owner'] }}]
-Repository Name       [{{ current_config['repo_name'] }}]
-Repository Branch     [{{ current_config['repo_branch'] }}]
+{% extends "base_config.html" %} {% block content %}
+***** [Chat] Chat *****
+OpenAI API key [{{ current_config['openai_api_key'] }}]
 *** You probably don't need to edit these. ***
-Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
-Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
-Submit
+Conversation Logfile [{{ current_config['conversation_logfile'] }}]
+Model                [{{ current_config['model'] }}]
+Chat Model           [{{ current_config['chat_model'] }}]
+Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/content_type_input.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,86 @@
-{% extends "base_data_integration.html" %}
+{% extends "base_config.html" %}
 {% block content %}
-<h2>{{ content_type }}</h2>
-<form id="config-form">
-    <div id="success" style="display: none;" ></div>
-    <table>
-        <tr>
-            <td>
-                <label for="input-files">Input Files</label>
-            </td>
-            <td id="input-files-cell">
-                {% if current_config['input_files'] is none %}
-                    <input type="text" id="input-files" name="input-files">
-                {% else %}
-                    {% for input_file in current_config['input_files'] %}
-                        <input type="text" id="input-files" name="input-files" value="{{ input_file }}">
-                    {% endfor %}
-                {% endif %}
-            </td>
-            <td>
-                <button type="button" id="input-files-button">Add</button>
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="input-filter">Input Filter</label>
-            </td>
-            <td id="input-filter-cell">
-                {% if current_config['input_filter'] is none %}
-                    <input type="text" id="input-filter" name="input-filter">
-                {% else %}
-                    {% for input_filter in current_config['input_filter'] %}
-                        <input type="text" id="input-filter" name="input-filter" value="{{ input_filter }}">
-                    {% endfor %}
-                {% endif %}
-            </td>
-            <td>
-                <button type="button" id="input-filter-button">Add</button>
-            </td>
-        </tr>
-    </table>
+<div class="page">
+    <div class="section">
+        <h2 class="section-title">
+            <img class="card-icon" src="/static/assets/icons/{{ content_type }}.svg" alt="{{ content_type|capitalize }}">
+            <span class="card-title-text">{{ content_type|capitalize }}</span>
+        </h2>
+        <form id="config-form">
+            <table>
+                <tr>
+                    <td>
+                        <label for="input-files">Input Files</label>
+                    </td>
+                    <td id="input-files-cell">
+                        {% if current_config['input_files'] is none %}
+                            <input type="text" id="input-files" name="input-files">
+                        {% else %}
+                            {% for input_file in current_config['input_files'] %}
+                                <input type="text" id="input-files" name="input-files" value="{{ input_file }}">
+                            {% endfor %}
+                        {% endif %}
+                    </td>
+                    <td>
+                        <button type="button" id="input-files-button">Add</button>
+                    </td>
+                </tr>
+                <tr>
+                    <td>
+                        <label for="input-filter">Input Filter</label>
+                    </td>
+                    <td id="input-filter-cell">
+                        {% if current_config['input_filter'] is none %}
+                            <input type="text" id="input-filter" name="input-filter">
+                        {% else %}
+                            {% for input_filter in current_config['input_filter'] %}
+                                <input type="text" id="input-filter" name="input-filter" value="{{ input_filter }}">
+                            {% endfor %}
+                        {% endif %}
+                    </td>
+                    <td>
+                        <button type="button" id="input-filter-button">Add</button>
+                    </td>
+                </tr>
+            </table>
 
-    <h4>You probably don't need to edit these.</h4>
+            <h4>You probably don't need to edit these.</h4>
 
-    <table>
-        <tr>
-            <td>
-                <label for="compressed-jsonl">Compressed JSONL (Output)</label>
-            </td>
-            <td>
-                <input type="text" id="compressed-jsonl" name="compressed-jsonl" value="{{ current_config['compressed_jsonl'] }}">
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="embeddings-file">Embeddings File (Output)</label>
-            </td>
-            <td>
-                <input type="text" id="embeddings-file" name="embeddings-file" value="{{ current_config['embeddings_file'] }}">
-            </td>
-        </tr>
-        <tr>
-            <td>
-                <label for="index-heading-entries">Index Heading Entries</label>
-            </td>
-            <td>
-                <input type="text" id="index-heading-entries" name="index-heading-entries" value="{{ current_config['index_heading_entries'] }}">
-            </td>
-        </tr>
-    </table>
-    <button id="submit" type="submit">Submit</button>
-</form>
+            <table>
+                <tr>
+                    <td>
+                        <label for="compressed-jsonl">Compressed JSONL (Output)</label>
+                    </td>
+                    <td>
+                        <input type="text" id="compressed-jsonl" name="compressed-jsonl" value="{{ current_config['compressed_jsonl'] }}">
+                    </td>
+                </tr>
+                <tr>
+                    <td>
+                        <label for="embeddings-file">Embeddings File (Output)</label>
+                    </td>
+                    <td>
+                        <input type="text" id="embeddings-file" name="embeddings-file" value="{{ current_config['embeddings_file'] }}">
+                    </td>
+                </tr>
+                <tr>
+                    <td>
+                        <label for="index-heading-entries">Index Heading Entries</label>
+                    </td>
+                    <td>
+                        <input type="text" id="index-heading-entries" name="index-heading-entries" value="{{ current_config['index_heading_entries'] }}">
+                    </td>
+                </tr>
+            </table>
+            <div id="success" style="display: none;" ></div>
+            <button id="submit" type="submit">Save</button>
+        </form>
+    </div>
+</div>
 <script>
     function addButtonEventListener(fieldName) {
         var button = document.getElementById(fieldName + "-button");
         button.addEventListener("click", function(event) {
             var cell = document.getElementById(fieldName + "-cell");
             var newInput = document.createElement("input");
             newInput.setAttribute("type", "text");
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-{% extends "base_data_integration.html" %} {% block content %}
-***** {{ content_type }} *****
+{% extends "base_config.html" %} {% block content %}
+***** [{{ content_type|capitalize }}] {{ content_type|capitalize }} *****
              {% if current_config['input_files'] is none %} [input-files
 Input Files  ] {% else %} {% for input_file in current_config              Add
              ['input_files'] %} [{{ input_file }}    ] {% endfor %} {%
              endif %}
              {% if current_config['input_filter'] is none %} [input-filter
 Input Filter ] {% else %} {% for input_filter in current_config            Add
              ['input_filter'] %} [{{ input_filter }}  ] {% endfor %} {%
              endif %}
 *** You probably don't need to edit these. ***
 Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
 Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
 Index Heading Entries     [{{ current_config['index_heading_entries'] }}]
-Submit
+Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/index.html` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,18 @@
     <head>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0 maximum-scale=1.0">
         <title>Khoj - Search</title>
 
         <link rel="icon" type="image/png" sizes="128x128" href="/static/assets/icons/favicon-128x128.png">
         <link rel="manifest" href="/static/khoj.webmanifest">
+        <link rel="stylesheet" href="/static/assets/khoj.css">
     </head>
-    <script type="text/javascript" src="static/assets/org.min.js"></script>
-    <script type="text/javascript" src="static/assets/markdown-it.min.js"></script>
+    <script type="text/javascript" src="/static/assets/org.min.js"></script>
+    <script type="text/javascript" src="/static/assets/markdown-it.min.js"></script>
 
     <script>
         function render_image(item) {
             return `
             <a href="${item.entry}" class="image-link">
                 <img id=${item.score} src="${item.entry}?${Math.random()}"
                     title="Effective Score: ${item.score}, Meta: ${item.additional.metadata_score}, Image: ${item.additional.image_score}"
@@ -184,17 +185,23 @@
             var query_via_url = new URLSearchParams(window.location.search).get("q");
             if (query_via_url)
                 document.getElementById("query").value = query_via_url;
         }
     </script>
 
     <body>
-        <h1>
-            <img class="khoj-logo" src="static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
-        </h1>
+        <!--Add Header Logo and Nav Pane-->
+        <div class="khoj-header">
+            <img class="khoj-logo" src="/static/assets/icons/khoj-logo-sideways.svg" alt="Khoj"></img>
+            <nav class="khoj-nav">
+                <a href="/chat">Chat</a>
+                <a class="khoj-nav-selected" href="/">Search</a>
+                <a href="/config">Settings</a>
+            </nav>
+        </div>
 
         <!--Add Text Box To Enter Query, Trigger Incremental Search OnChange -->
         <input type="text" id="query" class="option" onkeyup=incrementalSearch(event) autofocus="autofocus" placeholder="What is the meaning of life?">
 
         <div id="options">
             <!--Add Dropdown to Select Query Type -->
             <select id="type" class="option" onchange="setTypeFieldInUrl(this)"></select>
@@ -211,32 +218,31 @@
     </body>
 
     <style>
         @media only screen and (max-width: 600px) {
             body {
                 display: grid;
                 grid-template-columns: 1fr;
-                grid-template-rows: 1fr 1fr 1fr minmax(80px, 100%);
+                grid-template-rows: 1fr auto auto minmax(80px, 100%);
             }
             body > * {
                 grid-column: 1;
             }
         }
         @media only screen and (min-width: 600px) {
             body {
                 display: grid;
                 grid-template-columns: 1fr min(70vw, 100%) 1fr;
-                grid-template-rows: 1fr 1fr 1fr minmax(80px, 100%);
+                grid-template-rows: 1fr auto auto minmax(80px, 100%);
                 padding-top: 60vw;
             }
             body > * {
                 grid-column: 2;
             }
         }
-
         body {
             padding: 0px;
             margin: 0px;
             background: #f8fafc;
             color: #475569;
             text-align: center;
             font-family: roboto, karma, segoe ui, sans-serif;
@@ -244,22 +250,14 @@
             font-weight: 300;
             line-height: 1.5em;
         }
         body > * {
             padding: 10px;
             margin: 10px;
         }
-        h1 {
-            margin: 8px 0;
-            padding: 0;
-        }
-        img.khoj-logo {
-            width: min(60vw, 150px);
-        }
-
         #options {
             padding: 0;
             display: grid;
             grid-template-columns: 1fr 1fr minmax(70px, 0.5fr);
         }
         #options > * {
             padding: 15px;
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 
 
-****** [Khoj] ******
+
+[Khoj]  Chat Search Settings
  [                    ]
   Update  [Unknown INPUT type]
```

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.6.3.dev88/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/routers/api.py` & `khoj_assistant-0.6.3.dev88/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/routers/api_beta.py` & `khoj_assistant-0.6.3.dev88/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/routers/web_client.py` & `khoj_assistant-0.6.3.dev88/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.6.3.dev88/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.6.3.dev88/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.6.3.dev88/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/search_type/image_search.py` & `khoj_assistant-0.6.3.dev88/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/search_type/text_search.py` & `khoj_assistant-0.6.3.dev88/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/cli.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/config.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/constants.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/helpers.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/jsonl.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/models.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/state.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/src/khoj/utils/yaml.py` & `khoj_assistant-0.6.3.dev88/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/.gitignore` & `khoj_assistant-0.6.3.dev88/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/LICENSE` & `khoj_assistant-0.6.3.dev88/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/README.md` & `khoj_assistant-0.6.3.dev88/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/pyproject.toml` & `khoj_assistant-0.6.3.dev88/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.6.3.dev81/PKG-INFO` & `khoj_assistant-0.6.3.dev88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.6.3.dev81
+Version: 0.6.3.dev88
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

