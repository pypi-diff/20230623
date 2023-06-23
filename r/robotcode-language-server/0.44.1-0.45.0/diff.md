# Comparing `tmp/robotcode_language_server-0.44.1.tar.gz` & `tmp/robotcode_language_server-0.45.0.tar.gz`

## Comparing `robotcode_language_server-0.44.1.tar` & `robotcode_language_server-0.45.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    39560 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    58384 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    67010 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    85362 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.44.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21107 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19251 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    39564 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58494 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    68132 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    85362 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.45.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,15 +905,15 @@
 
     def _check_import_name(self, value: Optional[str], node: ast.AST, type: str) -> None:
         if not value:
             self.append_diagnostics(
                 range=range_from_node(node),
                 message=f"{type} setting requires value.",
                 severity=DiagnosticSeverity.ERROR,
-                code="ImportNeedsName",
+                code="ImportRequiresValue",
             )
 
     async def visit_VariablesImport(self, node: ast.AST) -> None:  # noqa: N802
         if get_robot_version() >= (6, 1):
             from robot.parsing.model.statements import VariablesImport
 
             import_node = cast(VariablesImport, node)
```

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,14 +567,15 @@
     def clear_cache(self) -> None:
         if self.cache_path.exists():
             shutil.rmtree(self.cache_path)
             self._logger.debug(lambda: f"Cleared cache {self.cache_path}")
 
     @_logger.call
     async def get_command_line_variables(self) -> List[VariableDefinition]:
+        from robot.errors import DataError
         from robot.utils.text import split_args_from_name_or_path
 
         async with self._command_line_variables_lock:
             if self._command_line_variables is None:
                 command_line_vars: List[VariableDefinition] = []
                 command_line_vars += [
                     CommandLineVariableDefinition(0, 0, 0, 0, "", f"${{{k}}}", None, has_value=True, value=v)
@@ -630,14 +631,16 @@
                                 for error in lib_doc.errors:
                                     self._logger.error(
                                         lambda: f"{error.type_name}: {error.message} in {error.source}:{error.line_no}"
                                     )
 
                     except (SystemExit, KeyboardInterrupt, asyncio.CancelledError):
                         raise
+                    except DataError:
+                        pass
                     except BaseException as e:
                         # TODO add diagnostics
                         self._logger.exception(e)
 
                 self._command_line_variables = command_line_vars
 
             return self._command_line_variables or []
```

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,14 +230,37 @@
     POSITIONAL_OR_NAMED = "POSITIONAL_OR_NAMED"
     VAR_POSITIONAL = "VAR_POSITIONAL"
     NAMED_ONLY_MARKER = "NAMED_ONLY_MARKER"
     NAMED_ONLY = "NAMED_ONLY"
     VAR_NAMED = "VAR_NAMED"
 
 
+def robot_arg_repr(arg: Any) -> Optional[str]:
+    from robot.running.arguments.argumentspec import ArgInfo
+
+    robot_arg = cast(ArgInfo, arg)
+
+    if robot_arg.default is ArgInfo.NOTSET:
+        return None
+
+    if robot_arg.default is None:
+        return "${None}"
+
+    if isinstance(robot_arg.default, (int, float, bool)):
+        return f"${{{robot_arg.default!r}}}"
+
+    if isinstance(robot_arg.default, str) and robot_arg.default == "":
+        return "${EMPTY}"
+
+    if isinstance(robot_arg.default, str) and robot_arg.default == "\\ \\":
+        return "${SPACE}"
+
+    return str(robot_arg.default_repr)
+
+
 @dataclass
 class KeywordArgumentDoc:
     name: str
     str_repr: str
     kind: KeywordArgumentKind
     required: bool
     default_value: Optional[Any] = None
@@ -247,23 +270,34 @@
     def from_robot(arg: Any) -> KeywordArgumentDoc:
         from robot.running.arguments.argumentspec import ArgInfo
 
         robot_arg = cast(ArgInfo, arg)
 
         return KeywordArgumentDoc(
             name=robot_arg.name,
-            default_value=robot_arg.default_repr,
+            default_value=robot_arg_repr(robot_arg),
             str_repr=str(arg),
             types=robot_arg.types_reprs,
             kind=KeywordArgumentKind[robot_arg.kind],
             required=robot_arg.required,
         )
 
     def __str__(self) -> str:
-        return self.str_repr
+        prefix = ""
+        if self.kind == KeywordArgumentKind.VAR_POSITIONAL:
+            prefix = "*"
+        elif self.kind == KeywordArgumentKind.VAR_NAMED:
+            prefix = "**"
+
+        return (
+            f"{prefix}{self.name!s}"
+            f"{(': ' + (' | '.join(f'{s}' for s in self.types))) if self.types else ''}"
+            f"{' =' if self.default_value is not None else ''}"
+            f"{f' {self.default_value!s}' if self.default_value else ''}"
+        )
 
     def __hash__(self) -> int:
         return id(self)
 
 
 DEPRECATED_PATTERN = re.compile(r"^\*DEPRECATED(?P<message>.*)\*(?P<doc>.*)")
 
@@ -427,15 +461,15 @@
         if add_signature:
             result += self._get_signature(header_level, add_type)
 
         if self.doc:
             if result:
                 result += "\n\n"
 
-            result += f"##{'#'*header_level} Documentation:\n\n"
+            result += f"##{'#'*header_level} Documentation:\n"
 
             if self.doc_format == ROBOT_DOC_FORMAT:
                 result += MarkDownFormatter().format(self.doc)
             elif self.doc_format == REST_DOC_FORMAT:
                 result += convert_from_rest(self.doc)
             else:
                 result += self.doc
@@ -448,31 +482,34 @@
         else:
             if not self.is_initializer:
                 result = f"\n\n#{'#'*header_level} {self.name}\n"
             else:
                 result = ""
 
         if self.args:
-            result += f"\n##{'#'*header_level} Arguments: \n\n"
+            result += f"\n##{'#'*header_level} Arguments: \n"
 
             result += "\n| | | | |"
-            result += "\n|:--- | --:|:--|:---|"
+            result += "\n|:--|:--|:--|:--|"
+
+            escaped_pipe = " \\| "
 
             for a in self.args:
                 prefix = ""
                 if a.kind == KeywordArgumentKind.VAR_POSITIONAL:
                     prefix = "*"
                 elif a.kind == KeywordArgumentKind.VAR_NAMED:
                     prefix = "**"
 
                 result += (
                     f"\n| `{prefix}{a.name!s}`"
-                    f"| {'=' if a.default_value is not None else ''}"
-                    f"| {f'`{a.default_value!s}`' if a.default_value else ''}"
-                    f"| {' or '.join(f'`<{s}>`' for s in a.types) if a.types is not None else ''} |"
+                    f'{": " if a.types else " "}'
+                    f"| {escaped_pipe.join(f'`{s}`' for s in a.types) if a.types else ''} "
+                    f"| {'=' if a.default_value is not None else ''} "
+                    f"| {f'`{a.default_value!s}`' if a.default_value else ''} |"
                 )
 
         if self.tags:
             if result:
                 result += "\n\n"
 
             result += "**Tags**: \n- "
@@ -701,15 +738,14 @@
             if add_signature and any(v for v in self.inits.values() if v.args):
                 for i in self.inits.values():
                     write_lines(i.to_markdown(header_level=header_level), "", "---")
 
             write_lines(
                 f"#{'#'*header_level} {(self.type.capitalize()) if self.type else 'Unknown'} *{self.name}*",
                 "",
-                "",
             )
 
             if self.version or self.scope:
                 write_lines(
                     "|  |  |",
                     "| :--- | :--- |",
                 )
```

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         from robot.parsing.model.statements import SectionHeader
 
         section = cast(Section, node)
         if section.header is None:
             return
 
         header = cast(SectionHeader, section.header)
-        if header.name is None:
+        if not header.name:
             return
 
         r = range_from_node(section)
         symbol = DocumentSymbol(
             name=header.name.replace("*", "").strip(),
             kind=SymbolKind.NAMESPACE,
             range=r,
```

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.45.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/.gitignore` & `robotcode_language_server-0.45.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/LICENSE.txt` & `robotcode_language_server-0.45.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/README.md` & `robotcode_language_server-0.45.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.44.1/pyproject.toml` & `robotcode_language_server-0.45.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.44.1",
-  "robotcode==0.44.1",
+  "robotcode-jsonrpc2==0.45.0",
+  "robotcode==0.45.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.44.1/PKG-INFO` & `robotcode_language_server-0.45.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.44.1
+Version: 0.45.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.44.1
-Requires-Dist: robotcode==0.44.1
+Requires-Dist: robotcode-jsonrpc2==0.45.0
+Requires-Dist: robotcode==0.45.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

