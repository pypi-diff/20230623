# Comparing `tmp/jupyterlab_quarto-0.1.45.tar.gz` & `tmp/jupyterlab_quarto-0.2.2.tar.gz`

## Comparing `jupyterlab_quarto-0.1.45.tar` & `jupyterlab_quarto-0.2.2.tar`

### file list

```diff
@@ -1,137 +1,117 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/.DS_Store
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/install.json
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jest.config.js
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/setup.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/tsconfig.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/.turbo/turbo-build.log
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/apa.csl
--rw-r--r--   0        0        0    99224 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/example.ipynb
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/palmer-biblio.bib
--rw-r--r--   0        0        0   212480 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/penguins.ipynb
--rw-r--r--   0        0        0    13431 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/working.jpeg
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/.ipynb_checkpoints/callouts-checkpoint.ipynb
--rw-r--r--   0        0        0    99258 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/.ipynb_checkpoints/example-checkpoint.ipynb
--rw-r--r--   0        0        0   212499 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/example/.ipynb_checkpoints/penguins-checkpoint.ipynb
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/_version.py
--rw-r--r--   0        0        0    21823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/build_log.json
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/package.json
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/schemas/jupyterlab-quarto/package.json.orig
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/schemas/jupyterlab-quarto/plugin.json
--rw-r--r--   0        0        0   141660 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/lib_index_js.9836512fdbbe11ebf7f6.js
--rw-r--r--   0        0        0   172521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/lib_index_js.9836512fdbbe11ebf7f6.js.map
--rw-r--r--   0        0        0    30920 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_css-loader_dist_cjs_js_style_base_css.cb83f33d662599046cd4.js
--rw-r--r--   0        0        0    33793 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_css-loader_dist_cjs_js_style_base_css.cb83f33d662599046cd4.js.map
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-deflist_index_js.0e6b0ffcf597c54b059b.js
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-deflist_index_js.0e6b0ffcf597c54b059b.js.map
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sub_index_js.1fff94f55b4e2916234e.js
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sub_index_js.1fff94f55b4e2916234e.js.map
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sup_index_js.a6cc7c1dd25e9485619c.js
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-sup_index_js.a6cc7c1dd25e9485619c.js.map
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-task-lists_index_js.63b640ba78c0f89e4ad7.js
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/node_modules_markdown-it-task-lists_index_js.63b640ba78c0f89e4ad7.js.map
--rw-r--r--   0        0        0    40940 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/remoteEntry.ecd67935a91a7a071575.js
--rw-r--r--   0        0        0    39743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/remoteEntry.ecd67935a91a7a071575.js.map
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/style.js
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/style_index_js.04d68d4fb5e2cadc4acc.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/style_index_js.04d68d4fb5e2cadc4acc.js.map
--rw-r--r--   0        0        0    12112 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6e87c73d7ee69f99abfd.js
--rw-r--r--   0        0        0    13811 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.6e87c73d7ee69f99abfd.js.map
--rw-r--r--   0        0        0   109159 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_js-yaml_dist_js-yaml_mjs.3c6d8dda6e87bd63f8fd.js
--rw-r--r--   0        0        0   130302 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_js-yaml_dist_js-yaml_mjs.3c6d8dda6e87bd63f8fd.js.map
--rw-r--r--   0        0        0    22926 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-attrs_index_js.ce676b74033540d8e3b2.js
--rw-r--r--   0        0        0    27484 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-attrs_index_js.ce676b74033540d8e3b2.js.map
--rw-r--r--   0        0        0    12043 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-footnote_index_js.6547d272bdd334cd78e2.js
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it-footnote_index_js.6547d272bdd334cd78e2.js.map
--rw-r--r--   0        0        0   212957 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_index_js.441a9acdab854e8f5e31.js
--rw-r--r--   0        0        0   237426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_index_js.441a9acdab854e8f5e31.js.map
--rw-r--r--   0        0        0    69731 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_lib_common_utils_js-node_modules_markdown-it_lib_token_js.fd3a84687ef0b7681712.js
--rw-r--r--   0        0        0    40156 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_markdown-it_lib_common_utils_js-node_modules_markdown-it_lib_token_js.fd3a84687ef0b7681712.js.map
--rw-r--r--   0        0        0  1554441 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_flowchart-elk-definition-170a3958_js.acad147ef8a8a7f9df1f.js
--rw-r--r--   0        0        0  2029534 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_flowchart-elk-definition-170a3958_js.acad147ef8a8a7f9df1f.js.map
--rw-r--r--   0        0        0  3481113 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mermaid_core_mjs.f1ecd3a98599231c8777.js
--rw-r--r--   0        0        0  3611887 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mermaid_core_mjs.f1ecd3a98599231c8777.js.map
--rw-r--r--   0        0        0  1216176 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mindmap-definition-44684416_js.4d34ed20a5d5a3bee971.js
--rw-r--r--   0        0        0  1472940 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_mindmap-definition-44684416_js.4d34ed20a5d5a3bee971.js.map
--rw-r--r--   0        0        0    55541 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_timeline-definition-8e5a9bc6_js.8e4504a1f9ebfe017e71.js
--rw-r--r--   0        0        0    68925 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_mermaid_dist_timeline-definition-8e5a9bc6_js.8e4504a1f9ebfe017e71.js.map
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_wcwidth_index_js.ae1a487a2058d8859c18.js
--rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/static/vendors-node_modules_wcwidth_index_js.ae1a487a2058d8859c18.js.map
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/schema/plugin.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/const.ts
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/index.ts
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/manager.ts
--rw-r--r--   0        0        0    61581 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/test.log
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/types.ts
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/widgets.ts
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-deflist.d.ts
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-footnote.d.ts
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-gridtables.d.ts
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-implicit-figures.d.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-sub.d.ts
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-sup.d.ts
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/@types/markdown-it-task-lists.d.ts
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/__tests__/myextension.spec.ts
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/ast/ast.ts
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/hooks/codemirror.ts
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/callouts.ts
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/cites.ts
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/decorator.ts
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/divs.ts
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/figure-divs.ts
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/figures.ts
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/math.ts
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/shortcodes.ts
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/spans.ts
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/table-captions.ts
--rw-r--r--   0        0        0    11854 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/yaml.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/index.ts
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/gridtables/GetCells.ts
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/EmitTable.ts
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/GetLine.ts
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/ParseTable.ts
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/interfaces/markdown-it/IState.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/gridtables/rules/gridtable.ts
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/mermaid/index.ts
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/utils/html.ts
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/utils/markdownit.ts
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/plugins/utils/tok.ts
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/attrs.ts
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/callouts.ts
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/cites.ts
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/decorator.ts
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/deflist.ts
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/divs.ts
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/figure-divs.ts
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/figures.ts
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/footnotes.ts
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/gridtables.ts
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/math.ts
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/mermaid.ts
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/provider.ts
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/shortcodes.ts
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/spans.ts
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/sub.ts
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/sup.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/table-captions.ts
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/tasklists.ts
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/src/providers/yaml.ts
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/style/index.js
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/LICENSE
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/README.md
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/.copier-answers.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/.yarnrc.yml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jest.config.js
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/tsconfig.test.json
+-rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/yarn.lock
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/_version.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/package.json
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/11.bbf21e9c517bec162b9c.js
+-rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/150.9b2f6283ffc934651e1c.js
+-rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/185.a8ca3522cb5c31423453.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
+-rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/316.f7e4dd762f98107da4a5.js
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/384.6c76694e25edf7010d50.js
+-rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/487.dee02fd512e9bb15dee6.js
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/543.40a7a1799fcad108039e.js
+-rw-r--r--   0        0        0    42379 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/573.79885c9e9fcb552239cd.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/573.79885c9e9fcb552239cd.js.LICENSE.txt
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/596.ef22233afe464ab9134a.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/645.406375856388e9d7e4e9.js
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/651.7673e27b3217024cb32d.js
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/700.30097f2c1808e10c985f.js
+-rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/724.265325864c2c7d67e29e.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
+-rw-r--r--   0        0        0    28851 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/923.7ebdae030f34ea336411.js
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/980.57fcdfda225b581383c0.js
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/remoteEntry.c22e74f8f6426ddbb410.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/style.js
+-rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/const.ts
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/index.ts
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/manager.ts
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/types.ts
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/widgets.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-deflist.d.ts
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-footnote.d.ts
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-gridtables.d.ts
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-implicit-figures.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-sub.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-sup.d.ts
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/@types/markdown-it-task-lists.d.ts
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/__tests__/jupyterlab_quarto.spec.ts
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/ast/ast.ts
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/hooks/codemirror.ts
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/callouts.ts
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/cites.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/decorator.ts
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/divs.ts
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/figure-divs.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/figures.ts
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/index.ts
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/math.ts
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/shortcodes.ts
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/spans.ts
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/table-captions.ts
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/yaml.ts
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/index.ts
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/gridtables/GetCells.ts
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/EmitTable.ts
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/GetLine.ts
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/ParseTable.ts
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/interfaces/markdown-it/IState.ts
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/gridtables/rules/gridtable.ts
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/mermaid/index.ts
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/utils/html.ts
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/utils/markdownit.ts
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/plugins/utils/tok.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/attrs.ts
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/callouts.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/cites.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/decorator.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/deflist.ts
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/divs.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/figure-divs.ts
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/figures.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/footnotes.ts
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/gridtables.ts
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/math.ts
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/mermaid.ts
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/provider.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/shortcodes.ts
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/spans.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/sub.ts
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/sup.ts
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/table-captions.ts
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/tasklists.ts
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/src/providers/yaml.ts
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/ui-tests/tests/jupyterlab_quarto.spec.ts
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/README.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.2/PKG-INFO
```

### Comparing `jupyterlab_quarto-0.1.45/RELEASE.md` & `jupyterlab_quarto-0.2.2/RELEASE.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-# Making a new release of jupyterlab-quarto
+# Making a new release of jupyterlab_quarto
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
-### Set the Version
+### Python package
 
-Bump the version using `hatch`. 
+This extension can be distributed as Python packages. All of the Python
+packaging instructions are in the `pyproject.toml` file to wrap your extension in a
+Python package. Before generating a package, you first need to install some tools:
 
 ```bash
-hatch version <new-version>
+pip install build twine hatch
 ```
 
-### Publish Source Extension to NPM
-
-To publish the source extension as a NPM package, do:
+Bump the version using `hatch`. By default this will create a tag.
+See the docs on [hatch-nodejs-version](https://github.com/agoose77/hatch-nodejs-version#semver) for details.
 
 ```bash
-npm login
-npm publish --access public
+hatch version <new-version>
 ```
 
-### Publish Prebuilt Extension to PyPi
-
-This extension can be distributed as Python
-packages. All of the Python
-packaging instructions in the `pyproject.toml` file to wrap your extension in a
-Python package. Before generating a package, we first need to install `build`.
+Make sure to clean up all the development files before building the package:
 
 ```bash
-pip install build twine hatch
+jlpm clean:all
 ```
 
-**Before building, note that you must temporarily update the `package.json` file to remove the `@quarto` prefix from the package name.**
+You could also clean up the local git repository:
+
+```bash
+git clean -dfX
+```
 
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 ```bash
-<update name in package.json to 'jupyterlab-quarto'>
-rm dist/*
-yarn build
 python -m build
-<update name in package.json to '@quarto/jupyterlab-quarto'>
 ```
 
 > `python setup.py sdist bdist_wheel` is deprecated and will not work for this package.
 
 Then to upload the package to PyPI, do:
 
 ```bash
 twine upload dist/*
 ```
 
+### NPM package
+
+To publish the frontend part of the extension as a NPM package, do:
+
+```bash
+npm login
+npm publish --access public
+```
+
 ## Automated releases with the Jupyter Releaser
 
 The extension repository should already be compatible with the Jupyter Releaser.
 
-Check out the [workflow documentation](https://github.com/jupyter-server/jupyter_releaser#typical-workflow) for more information.
+Check out the [workflow documentation](https://jupyter-releaser.readthedocs.io/en/latest/get_started/making_release_from_repo.html) for more information.
 
 Here is a summary of the steps to cut a new release:
 
-- Fork the [`jupyter-releaser` repo](https://github.com/jupyter-server/jupyter_releaser)
-- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the Github Secrets in the fork
+- Add `ADMIN_GITHUB_TOKEN`, `PYPI_TOKEN` and `NPM_TOKEN` to the [Github Secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets) in the repository
 - Go to the Actions panel
-- Run the "Draft Changelog" workflow
-- Merge the Changelog PR
-- Run the "Draft Release" workflow
-- Run the "Publish Release" workflow
+- Run the "Step 1: Prep Release" workflow
+- Check the draft changelog
+- Run the "Step 2: Publish Release" workflow
 
 ## Publishing to `conda-forge`
 
 If the package is not on conda forge yet, check the documentation to learn how to add it: https://conda-forge.org/docs/maintainer/adding_pkgs.html
 
 Otherwise a bot should pick up the new version publish to PyPI, and open a new PR on the feedstock repository automatically.
```

### Comparing `jupyterlab_quarto-0.1.45/package.json` & `jupyterlab_quarto-0.2.2/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.714405637254902%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/quarto-dev/jupyterlab-quarto/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/codemirror': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/apputils', '@jupyterlab/mainmenu', "*

 * *                   "'@jupyterlab/rendermime', '@jupyterlab/rendermime-interfaces', "*

 * *                   "'@jupyterlab/settingregistry', '@jupyterlab/ui-components', '@lumino/widgets', "*

 * *                   "'js-yaml']}",*

 * * "'devDependencies'": "{'@jupyterlab/ […]*

```diff
@@ -1,125 +1,191 @@
 {
     "author": {
         "email": "charles@posit.co",
         "name": "Charles Teague"
     },
     "bugs": {
-        "url": "https://github.com/quarto-dev/quarto/issues/"
+        "url": "https://github.com/quarto-dev/jupyterlab-quarto/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codemirror": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/rendermime-interfaces": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/widgets": "^1.37.1",
-        "js-yaml": "^4.1.0",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/codemirror": "^4.0.0",
         "markdown-it": "^12.2.3",
         "markdown-it-attrs": "^4.1.6",
         "markdown-it-deflist": "^2.0.3",
         "markdown-it-footnote": "^3.0.2",
         "markdown-it-implicit-figures": "^0.11.0",
         "markdown-it-sub": "^1.0.0",
         "markdown-it-sup": "^1.0.0",
         "markdown-it-task-lists": "^1.3.0",
         "mermaid": "^9.1.7",
         "wcwidth": "^1.0.1"
     },
     "description": "Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@types/codemirror": "5.60.5",
-        "@types/jest": "^26.0.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/codemirror": "^5.60.8",
+        "@types/d3": "^7.4.0",
+        "@types/dompurify": "^3.0.2",
+        "@types/jest": "^29.2.0",
+        "@types/js-yaml": "^4.0.5",
+        "@types/json-schema": "^7.0.11",
         "@types/markdown-it": "^12.2.3",
         "@types/markdown-it-attrs": "^4.1.0",
         "@types/mermaid": "^9.1.0",
+        "@types/react": "^18.0.26",
         "@types/wcwidth": "^1.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
-        "jest-environment-jsdom": "^26.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "jest": "^29.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
         "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
-        "typescript": "^4.9.4"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
+        }
+    },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts",
+        "tests",
+        "**/__tests__",
+        "ui-tests"
+    ],
     "files": [
-        "src/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
-    "homepage": "https://github.com/quarto-dev/quarto",
+    "homepage": "https://github.com/quarto-dev/jupyterlab-quarto",
     "jupyterlab": {
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
         "extension": true,
-        "outputDir": "jupyterlab-quarto/labextension",
-        "schemaDir": "schema"
+        "outputDir": "jupyterlab_quarto/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "jupyterlab-quarto",
+    "name": "jupyterlab_quarto",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/quarto-dev/quarto/quarto.git"
+        "url": "https://github.com/quarto-dev/jupyterlab-quarto.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab-quarto/labextension jupyterlab-quarto/_version.py",
+        "clean:labextension": "rimraf jupyterlab_quarto/labextension jupyterlab_quarto/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
-        "test": "jest",
+        "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "rules": {
+            "property-no-vendor-prefix": null,
+            "selector-class-pattern": null,
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "0.1.45"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_quarto-0.1.45/jupyterlab-quarto/labextension/schemas/jupyterlab-quarto/package.json.orig` & `jupyterlab_quarto-0.2.2/jupyterlab_quarto/labextension/package.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7118014705882354%*

 * *Differences: {"'bugs'": "{'url': 'https://github.com/quarto-dev/jupyterlab-quarto/issues'}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/codemirror': '^4.0.0', "*

 * *                   "delete: ['@jupyterlab/apputils', '@jupyterlab/mainmenu', "*

 * *                   "'@jupyterlab/rendermime', '@jupyterlab/rendermime-interfaces', "*

 * *                   "'@jupyterlab/settingregistry', '@jupyterlab/ui-components', '@lumino/widgets', "*

 * *                   "'js-yaml']}",*

 * * "'devDependencies'": "{'@jupyterlab/ […]*

```diff
@@ -1,125 +1,196 @@
 {
     "author": {
         "email": "charles@posit.co",
         "name": "Charles Teague"
     },
     "bugs": {
-        "url": "https://github.com/quarto-dev/quarto/issues/"
+        "url": "https://github.com/quarto-dev/jupyterlab-quarto/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codemirror": "^3.0.0",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/rendermime": "^3.0.0",
-        "@jupyterlab/rendermime-interfaces": "^3.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/widgets": "^1.37.1",
-        "js-yaml": "^4.1.0",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/codemirror": "^4.0.0",
         "markdown-it": "^12.2.3",
         "markdown-it-attrs": "^4.1.6",
         "markdown-it-deflist": "^2.0.3",
         "markdown-it-footnote": "^3.0.2",
         "markdown-it-implicit-figures": "^0.11.0",
         "markdown-it-sub": "^1.0.0",
         "markdown-it-sup": "^1.0.0",
         "markdown-it-task-lists": "^1.3.0",
         "mermaid": "^9.1.7",
         "wcwidth": "^1.0.1"
     },
     "description": "Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.1.0",
-        "@types/codemirror": "5.60.5",
-        "@types/jest": "^26.0.0",
+        "@jupyterlab/builder": "^4.0.0",
+        "@jupyterlab/testutils": "^4.0.0",
+        "@types/codemirror": "^5.60.8",
+        "@types/d3": "^7.4.0",
+        "@types/dompurify": "^3.0.2",
+        "@types/jest": "^29.2.0",
+        "@types/js-yaml": "^4.0.5",
+        "@types/json-schema": "^7.0.11",
         "@types/markdown-it": "^12.2.3",
         "@types/markdown-it-attrs": "^4.1.0",
         "@types/mermaid": "^9.1.0",
+        "@types/react": "^18.0.26",
         "@types/wcwidth": "^1.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.15.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "jest": "^26.0.0",
-        "jest-environment-jsdom": "^26.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "jest": "^29.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "stylelint": "^14.3.0",
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
         "stylelint-config-prettier": "^9.0.4",
-        "stylelint-config-recommended": "^6.0.0",
-        "stylelint-config-standard": "~24.0.0",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
         "stylelint-prettier": "^2.0.0",
-        "ts-jest": "^26.0.0",
-        "typescript": "^4.9.4"
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.0"
     },
+    "eslintConfig": {
+        "extends": [
+            "eslint:recommended",
+            "plugin:@typescript-eslint/eslint-recommended",
+            "plugin:@typescript-eslint/recommended",
+            "plugin:prettier/recommended"
+        ],
+        "parser": "@typescript-eslint/parser",
+        "parserOptions": {
+            "project": "tsconfig.json",
+            "sourceType": "module"
+        },
+        "plugins": [
+            "@typescript-eslint"
+        ],
+        "rules": {
+            "@typescript-eslint/no-explicit-any": "off",
+            "@typescript-eslint/no-namespace": "off",
+            "@typescript-eslint/no-unused-vars": [
+                "warn",
+                {
+                    "args": "none"
+                }
+            ],
+            "@typescript-eslint/no-use-before-define": "off",
+            "@typescript-eslint/quotes": [
+                "error",
+                "single",
+                {
+                    "allowTemplateLiterals": false,
+                    "avoidEscape": true
+                }
+            ],
+            "curly": [
+                "error",
+                "all"
+            ],
+            "eqeqeq": "error",
+            "prefer-arrow-callback": "error"
+        }
+    },
+    "eslintIgnore": [
+        "node_modules",
+        "dist",
+        "coverage",
+        "**/*.d.ts",
+        "tests",
+        "**/__tests__",
+        "ui-tests"
+    ],
     "files": [
-        "src/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
-        "schema/*.json"
+        "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
-    "homepage": "https://github.com/quarto-dev/quarto",
+    "homepage": "https://github.com/quarto-dev/jupyterlab-quarto",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.c22e74f8f6426ddbb410.js",
+            "style": "./style"
+        },
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
         "extension": true,
-        "outputDir": "jupyterlab-quarto/labextension",
-        "schemaDir": "schema"
+        "outputDir": "jupyterlab_quarto/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
-    "name": "jupyterlab-quarto",
+    "name": "jupyterlab_quarto",
+    "prettier": {
+        "arrowParens": "avoid",
+        "endOfLine": "auto",
+        "singleQuote": true,
+        "trailingComma": "none"
+    },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
-        "url": "https://github.com/quarto-dev/quarto/quarto.git"
+        "url": "https://github.com/quarto-dev/jupyterlab-quarto.git"
     },
     "scripts": {
         "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab-quarto/labextension jupyterlab-quarto/_version.py",
+        "clean:labextension": "rimraf jupyterlab_quarto/labextension jupyterlab_quarto/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:check": "jlpm prettier:base --check",
         "stylelint": "jlpm stylelint:check --fix",
         "stylelint:check": "stylelint --cache \"style/**/*.css\"",
-        "test": "jest",
+        "test": "jest --coverage",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
+    "stylelint": {
+        "extends": [
+            "stylelint-config-recommended",
+            "stylelint-config-standard",
+            "stylelint-prettier/recommended"
+        ],
+        "rules": {
+            "property-no-vendor-prefix": null,
+            "selector-class-pattern": null,
+            "selector-no-vendor-prefix": null,
+            "value-no-vendor-prefix": null
+        }
+    },
     "types": "lib/index.d.ts",
-    "version": "0.1.45"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/index.ts` & `jupyterlab_quarto-0.2.2/src/index.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 /*
-* index.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * index.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
+import {
+  IEditorLanguageRegistry,
+  IEditorThemeRegistry
+} from '@jupyterlab/codemirror';
+
 import { MarkdownItManager } from './types';
 import { mermaid } from './providers/mermaid';
 import { kMarkdownItMgr, kPackageNamespace } from './const';
 import { footnotes } from './providers/footnotes';
 
 import '../style/index.css';
 import { markdownItManager } from './manager';
@@ -34,19 +39,24 @@
 import { spans } from './providers/spans';
 import { shortcodes } from './providers/shortcodes';
 
 const plugin: JupyterFrontEndPlugin<MarkdownItManager> = {
   id: `${kPackageNamespace}:plugin`,
   autoStart: true,
   provides: kMarkdownItMgr,
-  activate: (_app: JupyterFrontEnd) => {
-    console.log('JupyterLab extension jupyterlab-quarto is activated!');
+  requires: [IEditorThemeRegistry, IEditorLanguageRegistry],
+  activate: (
+    _app: JupyterFrontEnd,
+    themeRegistry: IEditorThemeRegistry,
+    languageRegistry: IEditorLanguageRegistry
+  ) => {
+    console.log('JupyterLab extension jupyterlab_quarto is activated!');
 
-    // Create a markdown rendering manager 
-    return markdownItManager();
+    // Create a markdown rendering manager
+    return markdownItManager(themeRegistry, languageRegistry);
   }
 };
 
 // Markdown It Extensions which provide base Pandoc behavior
 const kPandocExtensions = [
   footnotes, // footnote seriously render in the cell in which they appear in :(
   spans,
@@ -69,10 +79,9 @@
   mermaid,
   callouts,
   decorator,
   yaml,
   shortcodes
 ];
 
-
 // The extensions that should be enabled for Jupyter
-export default [plugin, ...kPandocExtensions, ...kQuartoExtensions ];
+export default [plugin, ...kPandocExtensions, ...kQuartoExtensions];
```

### Comparing `jupyterlab_quarto-0.1.45/src/manager.ts` & `jupyterlab_quarto-0.2.2/src/manager.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,82 +1,105 @@
 /*
-* manager.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * manager.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 import { IRenderMime, markdownRendererFactory } from '@jupyterlab/rendermime';
-import { CodeMirrorEditor } from '@jupyterlab/codemirror';
+import {
+  IEditorLanguageRegistry,
+  IEditorThemeRegistry
+} from '@jupyterlab/codemirror';
 
 import MarkdownIt, { Options } from 'markdown-it';
 
 import { RenderedMarkdown } from './widgets';
 import { Hook, MarkdownItPluginProvider, Ranked, Renderer } from './types';
-import { codeMirrorHighlight, codeMirrorPreloadHook } from './hooks/codemirror';
+import {
+  codeMirrorHighlighter,
+  codeMirrorPreloadHook
+} from './hooks/codemirror';
 
 // Provides resolved MarkdownIt options using the passed in options, the plugin
 // options, and default options.
-const resolveOptions = (widget: RenderedMarkdown, options: Options, providers: MarkdownItPluginProvider[]) => {
+const resolveOptions = (
+  widget: RenderedMarkdown,
+  options: Options,
+  providers: MarkdownItPluginProvider[],
+  themeRegistry: IEditorThemeRegistry,
+  languageRegistry: IEditorLanguageRegistry
+) => {
   // Build options table
   let allOptions: Options = {
     html: true,
     linkify: true,
     typographer: true,
-    langPrefix: `cm-s-${CodeMirrorEditor.defaultConfig.theme} language-`,
-    highlight: codeMirrorHighlight
+    langPrefix: `cm-s-${themeRegistry.defaultTheme} language-`,
+    highlight: codeMirrorHighlighter(languageRegistry)
   };
   for (const plugin of providers) {
     if (plugin.options) {
       try {
         // Add options for this plugin
         allOptions = { ...allOptions, ...plugin.options(widget) };
       } catch (err) {
-        console.warn(`Failed to get options from markdown-it plugin ${plugin.id}`, err);
-      }  
+        console.warn(
+          `Failed to get options from markdown-it plugin ${plugin.id}`,
+          err
+        );
+      }
     }
   }
 
   return {
     ...allOptions,
-    ...options };
-}
-
-export function markdownItManager() {
+    ...options
+  };
+};
 
+export function markdownItManager(
+  themeRegistry: IEditorThemeRegistry,
+  languageRegistry: IEditorLanguageRegistry
+) {
   // The plugin providers
   const pluginProviders: Map<string, MarkdownItPluginProvider> = new Map();
 
   //  The IMarkdownItManager
   const manager = {
     registerPlugin(provider: MarkdownItPluginProvider): void {
       pluginProviders.set(provider.id, provider);
     },
 
     async getRenderer(
       widget: RenderedMarkdown,
       options: Options = {}
     ): Promise<Renderer> {
-  
       // Fetch the list of providers
       const providers = [...pluginProviders.values()];
       providers.sort(sortRanked);
-  
+
       // Create MarkdownIt instance
-      const allOptions = resolveOptions(widget, options, providers);
+      const allOptions = resolveOptions(
+        widget,
+        options,
+        providers,
+        themeRegistry,
+        languageRegistry
+      );
       let md = new MarkdownIt('default', allOptions);
-  
+
       // Lifecycle hooks
       const preParseHooks: Hook<string, string>[] = [];
       const postRenderHooks: Hook<HTMLElement, void>[] = [];
 
       // add mode pre-loading hook if using default highlighter
-      if (codeMirrorHighlight === allOptions.highlight) {
-        preParseHooks.push(codeMirrorPreloadHook());
+      if (codeMirrorHighlighter(languageRegistry) === allOptions.highlight) {
+        preParseHooks.push(codeMirrorPreloadHook(languageRegistry));
       }
-  
+
       // Build MarkdownIt and load lifecycle hooks
       for (const provider of providers) {
         try {
           // Load MarkdownIt plugin
           const [plugin, ...pluginOptions] = await provider.plugin();
 
           // Build MarkdownIt instance
@@ -86,26 +109,28 @@
           if (provider.hooks?.preParse !== undefined) {
             preParseHooks.push(provider.hooks?.preParse);
           }
           if (provider.hooks?.postRender !== undefined) {
             postRenderHooks.push(provider.hooks?.postRender);
           }
         } catch (err) {
-          console.warn(`Failed to load/use markdown-it plugin ${provider.id}`, err);
+          console.warn(
+            `Failed to load/use markdown-it plugin ${provider.id}`,
+            err
+          );
         }
       }
       // Sort hooks by rank
       preParseHooks.sort(sortRanked);
       postRenderHooks.sort(sortRanked);
 
       return {
-
         // Parse and render Markdown
-        render: (content) => {
-          return md.render(content)
+        render: content => {
+          return md.render(content);
         },
 
         // Run hooks serially
         preParse: async (content: string) => {
           for (const hook of preParseHooks) {
             content = await hook.run(content);
           }
@@ -116,23 +141,24 @@
         postRender: async (node: HTMLElement) => {
           for (const hook of postRenderHooks) {
             await hook.run(node);
           }
         }
       };
     }
-  }
+  };
 
   // Register the Renderer
-  markdownRendererFactory.createRenderer = (options: IRenderMime.IRendererOptions) => {
+  markdownRendererFactory.createRenderer = (
+    options: IRenderMime.IRendererOptions
+  ) => {
     return new RenderedMarkdown(options, manager);
   };
-  
+
   return manager;
 }
 
-
 // Sorts by rank, using 100 if no default is provided.
 const kDefaultRank = 100;
 const sortRanked = (left: Ranked, right: Ranked) => {
   return (left.rank ?? kDefaultRank) - (right.rank ?? kDefaultRank);
-}
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/types.ts` & `jupyterlab_quarto-0.2.2/src/types.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 /*
-* types.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * types.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 import MarkdownIt from 'markdown-it';
 import { RenderedMarkdown } from './widgets';
 import { IRenderMime } from '@jupyterlab/rendermime-interfaces';
 import { ISanitizer } from '@jupyterlab/apputils';
 
-
 // Manages MarkdownIt Plugins
 export interface MarkdownItManager {
   registerPlugin(provider: MarkdownItPluginProvider): void;
 
   getRenderer(
     widget: RenderedMarkdown,
     options?: MarkdownIt.Options
@@ -42,22 +41,22 @@
   // A lazy provider of the plugin function and plugin options
   plugin(): Promise<[MarkdownItPlugin, ...any]>;
 
   // Additional options to pass to the MarkdownIt constructor
   options?(widget: RenderedMarkdown): Partial<MarkdownIt.Options>;
 
   // Hooks called during the various Markdown rendering phases
-  hooks?: { 
+  hooks?: {
     // Source transformer hook, invoked before Markdown parsing
     preParse?: Hook<string, string>;
 
     // Modifier hook, invoked after rendered Markdown
     // has been added to the DOM
     postRender?: Hook<HTMLElement, void>;
-  }
+  };
 }
 
 export interface RenderOptions {
   // The host node for the rendered Markdown.
   host: HTMLElement;
 
   // The Markdown source to render.
@@ -82,15 +81,14 @@
   renderer: Renderer;
 
   // The LaTeX typesetter for the application.
   latexTypesetter: IRenderMime.ILatexTypesetter | null;
 }
 
 export interface Renderer {
-
   // render content to HTML
   render(content: string): string;
 
   // Work on the pre-parsed markdown
   preParse(node: string): Promise<string>;
 
   // Work on the rendered HTML
```

### Comparing `jupyterlab_quarto-0.1.45/src/widgets.ts` & `jupyterlab_quarto-0.2.2/src/widgets.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 /*
-* widgets.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * widgets.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 import { RenderedHTMLCommon, renderHTML } from '@jupyterlab/rendermime';
 import { IRenderMime } from '@jupyterlab/rendermime-interfaces';
 import { Message } from '@lumino/messaging';
 import { MarkdownItManager, Renderer } from './types';
 
 // A mime rendered that renders Quarto Markdown
 export class RenderedMarkdown extends RenderedHTMLCommon {
-  
-  constructor(options: IRenderMime.IRendererOptions, manager: MarkdownItManager) {
+  constructor(
+    options: IRenderMime.IRendererOptions,
+    manager: MarkdownItManager
+  ) {
     super(options);
     this.addClass('quarto-rendered-md');
     this.markdownItManager = manager;
   }
   private markdownItManager: MarkdownItManager;
 
   // Renders a mime model
@@ -35,21 +37,21 @@
       shouldTypeset: this.isAttached,
       renderer: this.renderer,
       latexTypesetter: this.latexTypesetter
     };
 
     // Transform source
     const markup = await renderer.preParse(source);
-  
+
     // Clear the content if there is no source.
     if (!markup) {
       host.textContent = '';
       return;
     }
-  
+
     // Render HTML.
     await renderHTML({
       host,
       source: renderer.render(markup),
       ...others,
       shouldTypeset: false
     });
```

### Comparing `jupyterlab_quarto-0.1.45/src/ast/ast.ts` & `jupyterlab_quarto-0.2.2/src/ast/ast.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-import type Token from "markdown-it/lib/token"
+import type Token from 'markdown-it/lib/token';
 
 export const toAst = (toks: Token[]) => {
-    let pos = 0;
-    const inner = () => {
-        if (pos >= toks.length) return;
-        const tok = toks[pos];
-        if (tok.type.endsWith('_open')) {
-            ++pos;
-            const children: any[] = [];
-            while (toks[pos].type !== tok.type.replace('_open', '_close')) {
-                children.push(inner());
-            }
-            ++pos;
-            return {
-                ...tok,
-                type: tok.type.replace('_open', ''),
-                children: children
-            } as Token;
-        }
-        if (tok.type === 'inline' && tok.children) {
-            const children = toAst(tok.children);
-            ++pos;
-            return {
-                ...tok,
-                children
-            } as Token;
-        }
-        ++pos;
-        return tok;
+  let pos = 0;
+  const inner = () => {
+    if (pos >= toks.length) {
+      return;
     }
-    const result: Token[] = [];
-    while (pos < toks.length) {
-        const node = inner();
-        if (node) result.push(node);
+    const tok = toks[pos];
+    if (tok.type.endsWith('_open')) {
+      ++pos;
+      const children: any[] = [];
+      while (toks[pos].type !== tok.type.replace('_open', '_close')) {
+        children.push(inner());
+      }
+      ++pos;
+      return {
+        ...tok,
+        type: tok.type.replace('_open', ''),
+        children: children
+      } as Token;
     }
-    return result;
+    if (tok.type === 'inline' && tok.children) {
+      const children = toAst(tok.children);
+      ++pos;
+      return {
+        ...tok,
+        children
+      } as Token;
+    }
+    ++pos;
+    return tok;
+  };
+  const result: Token[] = [];
+  while (pos < toks.length) {
+    const node = inner();
+    if (node) {
+      result.push(node);
+    }
+  }
+  return result;
 };
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/callouts.ts` & `jupyterlab_quarto-0.2.2/src/plugins/callouts.ts`

 * *Files 19% similar despite different names*

```diff
@@ -1,258 +1,263 @@
 /*
-* callouts.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
-import type MarkdownIt from "markdown-it/lib"
-import Renderer from "markdown-it/lib/renderer";
-import Token from "markdown-it/lib/token";
-import { addClass, readAttrValue } from "./utils/markdownit";
-import { kTokDivClose, kTokDivOpen } from "./divs";
-
-
-const kTokCalloutOpen = "quarto_callout_open";
-const kTokCalloutClose = "quarto_callout_close";
+ * callouts.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
+import type MarkdownIt from 'markdown-it/lib';
+import Renderer from 'markdown-it/lib/renderer';
+import Token from 'markdown-it/lib/token';
+import { addClass, readAttrValue } from './utils/markdownit';
+import { kTokDivClose, kTokDivOpen } from './divs';
+
+const kTokCalloutOpen = 'quarto_callout_open';
+const kTokCalloutClose = 'quarto_callout_close';
 
-const kTokCalloutTitleOpen = "quarto_callout_title_open";
-const kTokCalloutTitleClose = "quarto_callout_title_close";
+const kTokCalloutTitleOpen = 'quarto_callout_title_open';
+const kTokCalloutTitleClose = 'quarto_callout_title_close';
 
-const kTokCalloutContentOpen = "quarto_callout_content_open";
-const kTokCalloutContentClose = "quarto_callout_content_close";
+const kTokCalloutContentOpen = 'quarto_callout_content_open';
+const kTokCalloutContentClose = 'quarto_callout_content_close';
 
-const kCalloutPrefix = "callout-";
-const kCalloutRuleName = "quarto-callouts";
+const kCalloutPrefix = 'callout-';
+const kCalloutRuleName = 'quarto-callouts';
 
 interface Callout {
-  type: "note" | "caution" | "warning" | "important" | "tip" | string;
+  type: 'note' | 'caution' | 'warning' | 'important' | 'tip' | string;
   clz: string;
   title?: string;
   icon?: boolean;
-  appearance?: "default" | "minimal" | "simple";
+  appearance?: 'default' | 'minimal' | 'simple';
   collapse?: boolean;
-} 
+}
 
 export const calloutPlugin = (md: MarkdownIt) => {
-  
   // Handle pandoc-style divs
-  md.core.ruler.push(
-    kCalloutRuleName,
-    (state) => {
-      const noteStartCallout = (callout: Callout, depth: number) => {
-        if (calloutDepth == -1) {
-          calloutDepth = depth;
-        }
-        state.env['quarto-active-callout'] = callout;
-      }
-
-      const noteCloseCallout = () => {
-        calloutDepth = -1;
-        state.env['quarto-active-callout'] = undefined;
-      }
-
-      const activeCallout = () => {
-        return state.env['quarto-active-callout'];
-      }
-
-      const isCloseCallout = (depth: number) => {
-        return calloutDepth === depth;
+  md.core.ruler.push(kCalloutRuleName, state => {
+    const noteStartCallout = (callout: Callout, depth: number) => {
+      if (calloutDepth === -1) {
+        calloutDepth = depth;
       }
+      state.env['quarto-active-callout'] = callout;
+    };
 
-      const titleOpenTok = (title?: string) => {
-        const token = new Token(kTokCalloutTitleOpen, "", 1)
-        token.tag = "div";
-        token.attrs = [["class", "callout-header"]];
-        if (title) {
-          token.attrs.push(["title", title]);
-        }
-        return token;
+    const noteCloseCallout = () => {
+      calloutDepth = -1;
+      state.env['quarto-active-callout'] = undefined;
+    };
+
+    const activeCallout = () => {
+      return state.env['quarto-active-callout'];
+    };
+
+    const isCloseCallout = (depth: number) => {
+      return calloutDepth === depth;
+    };
+
+    const titleOpenTok = (title?: string) => {
+      const token = new Token(kTokCalloutTitleOpen, '', 1);
+      token.tag = 'div';
+      token.attrs = [['class', 'callout-header']];
+      if (title) {
+        token.attrs.push(['title', title]);
       }
+      return token;
+    };
 
-      const titleCloseTok = () => {
-        const token = new Token(kTokCalloutTitleClose, "", -1)
-        token.tag = "div";
-        return token;       
-      }
-
-      const contentOpenTok = () => {
-        const token = new Token(kTokCalloutContentOpen, "", 1)
-        token.tag = "div";
-        token.attrs = [["class", "callout-body-container callout-body"]];
-        return token;
-      }
-
-      const contentCloseTok = () => {
-        const token = new Token(kTokCalloutContentClose, "", -1)
-        token.tag = "div";
-        return token;        
-      }
-
-      const outTokens: Token[] = [];
-      let calloutDepth = -1;
-      let divDepth = 0;
-      // just started callout - process title
-      // finished processing title - process content
-
-      let calloutState: "scanning" | "add-title" | "capturing-title" | "add-body" | "capturing-body" =  "scanning";
-      for (const token of state.tokens) {
-
-        switch (calloutState) {
-          case "add-title":
-            if (token.type === "heading_open") {
-              outTokens.push(titleOpenTok()); 
-              calloutState = "capturing-title";
-            } else {
-              const callout = activeCallout();
-              outTokens.push(titleOpenTok(callout.title)); 
-              outTokens.push(titleCloseTok()); 
-              calloutState = "add-body";
-            }
-            break;
-          case "capturing-title":
-            if (token.type === "heading_close") {
-              outTokens.push(titleCloseTok()); 
-              calloutState = "add-body";
+    const titleCloseTok = () => {
+      const token = new Token(kTokCalloutTitleClose, '', -1);
+      token.tag = 'div';
+      return token;
+    };
+
+    const contentOpenTok = () => {
+      const token = new Token(kTokCalloutContentOpen, '', 1);
+      token.tag = 'div';
+      token.attrs = [['class', 'callout-body-container callout-body']];
+      return token;
+    };
+
+    const contentCloseTok = () => {
+      const token = new Token(kTokCalloutContentClose, '', -1);
+      token.tag = 'div';
+      return token;
+    };
+
+    const outTokens: Token[] = [];
+    let calloutDepth = -1;
+    let divDepth = 0;
+    // just started callout - process title
+    // finished processing title - process content
+
+    let calloutState:
+      | 'scanning'
+      | 'add-title'
+      | 'capturing-title'
+      | 'add-body'
+      | 'capturing-body' = 'scanning';
+    for (const token of state.tokens) {
+      switch (calloutState) {
+        case 'add-title':
+          if (token.type === 'heading_open') {
+            outTokens.push(titleOpenTok());
+            calloutState = 'capturing-title';
+          } else {
+            const callout = activeCallout();
+            outTokens.push(titleOpenTok(callout.title));
+            outTokens.push(titleCloseTok());
+            calloutState = 'add-body';
+          }
+          break;
+        case 'capturing-title':
+          if (token.type === 'heading_close') {
+            outTokens.push(titleCloseTok());
+            calloutState = 'add-body';
+          } else {
+            outTokens.push(token);
+          }
+          break;
+        case 'add-body':
+          outTokens.push(contentOpenTok());
+          outTokens.push(token);
+          calloutState = 'capturing-body';
+          break;
+        case 'scanning':
+        default:
+          if (token.type === kTokDivOpen) {
+            divDepth++;
+            const callout = parseCallout(token.attrs);
+            if (callout) {
+              noteStartCallout(callout, divDepth);
+              calloutState = 'add-title';
+
+              const openCallout = new Token(kTokCalloutOpen, '', 1);
+              openCallout.attrs = openCallout.attrs || [];
+              openCallout.meta = callout;
+              outTokens.push(openCallout);
             } else {
               outTokens.push(token);
             }
-            break;
-          case "add-body":
-            outTokens.push(contentOpenTok());
-            outTokens.push(token);
-            calloutState = "capturing-body";
-            break;
-          case "scanning":
-          default:
-            if (token.type === kTokDivOpen) {
-              divDepth++;
-              const callout = parseCallout(token.attrs);
-              if (callout) {
-                noteStartCallout(callout, divDepth);
-                calloutState = "add-title";
-              
-                const openCallout = new Token(kTokCalloutOpen, "", 1);
-                openCallout.attrs = openCallout.attrs || [];
-                openCallout.meta = callout;
-                outTokens.push(openCallout);
-              } else {
-                outTokens.push(token);
-              }
-            } else if (token.type === kTokDivClose) {   
-              if (isCloseCallout(divDepth)) {
-                outTokens.push(contentCloseTok());
-                outTokens.push(new Token(kTokCalloutClose, "", -1));
-                noteCloseCallout()
-              } else {
-                outTokens.push(token);
-              }
-              divDepth--;
-              
+          } else if (token.type === kTokDivClose) {
+            if (isCloseCallout(divDepth)) {
+              outTokens.push(contentCloseTok());
+              outTokens.push(new Token(kTokCalloutClose, '', -1));
+              noteCloseCallout();
             } else {
               outTokens.push(token);
             }
-            break;
-        }
+            divDepth--;
+          } else {
+            outTokens.push(token);
+          }
+          break;
       }
-      state.tokens = outTokens;
-      return false;
     }
-  )
-  md.renderer.rules[kTokCalloutOpen] = renderStartCallout
-  md.renderer.rules[kTokCalloutClose] = renderEndCallout
-  md.renderer.rules[kTokCalloutTitleOpen] = renderStartCalloutTitle
-  md.renderer.rules[kTokCalloutTitleClose] = renderEndCalloutTitle
-}
-
+    state.tokens = outTokens;
+    return false;
+  });
+  md.renderer.rules[kTokCalloutOpen] = renderStartCallout;
+  md.renderer.rules[kTokCalloutClose] = renderEndCallout;
+  md.renderer.rules[kTokCalloutTitleOpen] = renderStartCalloutTitle;
+  md.renderer.rules[kTokCalloutTitleClose] = renderEndCalloutTitle;
+};
 
 // Render pandoc-style divs
-function renderStartCallout(tokens: Token[], idx: number, _options: MarkdownIt.Options, _env: unknown, self: Renderer): string {
+function renderStartCallout(
+  tokens: Token[],
+  idx: number,
+  _options: MarkdownIt.Options,
+  _env: unknown,
+  self: Renderer
+): string {
   const token = tokens[idx];
   const callout = token.meta as Callout;
 
   // Add classes decorating as callout
   token.attrs = addClass(`callout ${callout.clz}`, token.attrs);
 
   // Add class that reflects the style
   token.attrs = addClass(appearanceClass(callout.appearance), token.attrs);
 
   return `<div ${self.renderAttrs(token)}>`;
 }
 
 // Render pandoc-style divs
 function renderEndCallout(): string {
-  return `</div>`;
+  return '</div>';
 }
 
 function renderStartCalloutTitle(tokens: Token[], idx: number): string {
   const token = tokens[idx];
-  const title = readAttrValue("title", token.attrs) || "";
+  const title = readAttrValue('title', token.attrs) || '';
   const startContent = `
 <div class="callout-header">
 <div class="callout-icon-container">
   <i class="callout-icon"></i>
 </div>
 <div class="callout-title-container">${title}
 `;
   return startContent;
 }
 
 function renderEndCalloutTitle(): string {
-  return `</div>\n</div>`;
+  return '</div>\n</div>';
 }
 
-
 const calloutAppearance = (val: string | undefined) => {
   if (val) {
-    switch(val) {
-      case "minimal":
-        return "minimal";
-      case "simple":
-        return "simple"
-      case "default":
+    switch (val) {
+      case 'minimal':
+        return 'minimal';
+      case 'simple':
+        return 'simple';
+      case 'default':
       default:
-        return "default";
+        return 'default';
     }
   } else {
-    return "default";
+    return 'default';
   }
-}
+};
 
-const parseCallout = (attrs: null | [string, string][]) : Callout | undefined => {
-  if (attrs === null) { 
+const parseCallout = (
+  attrs: null | [string, string][]
+): Callout | undefined => {
+  if (attrs === null) {
     return undefined;
   }
 
-  const classAttr = attrs.find((attr) => { return attr[0] === "class"});
+  const classAttr = attrs.find(attr => {
+    return attr[0] === 'class';
+  });
   if (!classAttr) {
     return undefined;
   }
 
-  const classes = classAttr[1].split(" ");
-  const calloutClass = classes.find((clz) => {
+  const classes = classAttr[1].split(' ');
+  const calloutClass = classes.find(clz => {
     return clz.startsWith('callout-');
-  })
+  });
 
-  if (calloutClass) { 
-    const type = calloutClass.replace(kCalloutPrefix, "")
-    
-    const title = readAttrValue("title", attrs) || type.slice(0, 1).toUpperCase() + type.slice(1);;
-    const appearance = calloutAppearance(readAttrValue("appearance", attrs));
+  if (calloutClass) {
+    const type = calloutClass.replace(kCalloutPrefix, '');
+
+    const title =
+      readAttrValue('title', attrs) ||
+      type.slice(0, 1).toUpperCase() + type.slice(1);
+    const appearance = calloutAppearance(readAttrValue('appearance', attrs));
 
     return {
-      type: type || "note",
+      type: type || 'note',
       clz: calloutClass,
       title,
       appearance
-    }
-
+    };
   } else {
     return undefined;
   }
+};
 
-}
-
-const appearanceClass = (appearance?:  "default" | "minimal" | "simple") => {
-  const style = appearance || "default";
+const appearanceClass = (appearance?: 'default' | 'minimal' | 'simple') => {
+  const style = appearance || 'default';
   return `callout-style-${style}`;
-}
-
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/cites.ts` & `jupyterlab_quarto-0.2.2/src/plugins/cites.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,160 @@
 /*
-* citation.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * citation.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
+
+import type MarkdownIt from 'markdown-it/lib';
+import Renderer from 'markdown-it/lib/renderer';
+import Token from 'markdown-it/lib/token';
 
-
-import type MarkdownIt from "markdown-it/lib"
-import Renderer from "markdown-it/lib/renderer";
-import Token from "markdown-it/lib/token";
-
-const kTokCite = "quarto_cite";
+const kTokCite = 'quarto_cite';
 
 export const citationPlugin = (md: MarkdownIt) => {
-
   // Very simple plugin example that surrounds @text with `code`
-  md.core.ruler.push('quarto-citation', function replaceAtSymbol(state) {
+  md.core.ruler.push('quarto-citation', state => {
     const tokens = state.tokens;
 
     for (const token of tokens) {
       if (token.type === 'inline' && token.children) {
-
         // Rebuild the child list
         const children: Token[] = [];
         for (let i = 0; i < token.children.length; i++) {
           const child = token.children[i];
           if (child.type === 'text') {
             const content = child.content;
 
-
             const textToken = (text: string[]) => {
               const newToken = new state.Token('text', '', 0);
-              newToken.content = text.join("");
-              
+              newToken.content = text.join('');
+
               return newToken;
-            }
+            };
 
             let text: string[] = [];
             const flushText = () => {
               if (text.length) {
                 children.push(textToken(text));
-                text = [];                  
+                text = [];
               }
-            }
+            };
 
             let cite: string[] = [];
             const flushCite = () => {
               if (cite.length) {
                 // Determine the cite style
-                let style = cite[0] === "-" ? "suppress-author" : "in-text";
+                let style = cite[0] === '-' ? 'suppress-author' : 'in-text';
                 if (bracketCount > 0) {
-                  style = "normal";
+                  style = 'normal';
                 }
 
                 // The classes
-                const clz = ["cite", style];
+                const clz = ['cite', style];
 
                 // If the cite ends in punctuation, trim that off and make that text
                 const puncText: string[] = [];
 
                 // Trim off ending punctuation
-                if ([":",".","#","$","%","&","-","+","?","<",">","~","/","!"].includes(cite[cite.length - 1])) {
+                if (
+                  [
+                    ':',
+                    '.',
+                    '#',
+                    '$',
+                    '%',
+                    '&',
+                    '-',
+                    '+',
+                    '?',
+                    '<',
+                    '>',
+                    '~',
+                    '/',
+                    '!'
+                  ].includes(cite[cite.length - 1])
+                ) {
                   puncText.push(cite[cite.length - 1]);
                   cite = cite.slice(0, -1);
                 }
 
                 // Make a cite token
                 const newToken = new state.Token(kTokCite, '', 0);
-                newToken.content = cite.join("");
+                newToken.content = cite.join('');
                 newToken.attrs = newToken.attrs || [];
-                newToken.attrs?.push(["class", clz.join(" ")]);
+                newToken.attrs?.push(['class', clz.join(' ')]);
                 children.push(newToken);
-                cite = []; 
-                
+                cite = [];
+
                 if (puncText.length > 0) {
                   children.push(textToken(puncText));
                 }
               }
-            }
+            };
 
-            let capture: "text" | "cite" = "text";
+            let capture: 'text' | 'cite' = 'text';
             let bracketCount = 0;
             for (let j = 0; j < content.length; j++) {
-
               const char = content.charAt(j);
-              if (char === "@") {
-                if ((text.length === 1 && text[0] === '-') || 
-                    text.length > 1 && text[text.length - 1] === "-" && text[text.length - 2] === "[") {
+              if (char === '@') {
+                if (
+                  (text.length === 1 && text[0] === '-') ||
+                  (text.length > 1 &&
+                    text[text.length - 1] === '-' &&
+                    text[text.length - 2] === '[')
+                ) {
                   cite.push('-');
                   cite.push(char);
                   text.pop();
                   flushText();
                   capture = 'cite';
                 } else if (text[text.length - 1] === ' ') {
-                  flushText();   
+                  flushText();
                   cite.push(char);
-                  capture = 'cite';               
-                } else if (text[text.length- 1] === '-' && text[text.length - 2] === ' ') {
+                  capture = 'cite';
+                } else if (
+                  text[text.length - 1] === '-' &&
+                  text[text.length - 2] === ' '
+                ) {
                   text = text.slice(0, -1);
                   flushText();
                   cite.push('-');
                   cite.push(char);
                   capture = 'cite';
-                } else if (text[text.length - 1] === '[' && text[text.length - 2] === ' ') {
+                } else if (
+                  text[text.length - 1] === '[' &&
+                  text[text.length - 2] === ' '
+                ) {
                   flushText();
                   cite.push(char);
                   capture = 'cite';
                 } else if (text.length === 0) {
                   cite.push(char);
                   capture = 'cite';
-                }
-                else {
+                } else {
                   if (capture === 'cite') {
                     cite.push(char);
                   } else {
                     text.push(char);
-                  }  
+                  }
                 }
-              } else if (char === " ") { 
+              } else if (char === ' ') {
                 capture = 'text';
                 flushCite();
                 text.push(char);
-              } else if (char === "[") {
+              } else if (char === '[') {
                 bracketCount++;
                 text.push(char);
-              } else if (char === "]") {
+              } else if (char === ']') {
                 bracketCount--;
                 capture = 'text';
                 flushCite();
                 text.push(char);
-              }
-              else {
+              } else {
                 if (capture === 'cite') {
                   cite.push(char);
                 } else {
                   text.push(char);
                 }
               }
             }
@@ -145,17 +165,24 @@
           }
         }
         token.children = children.length > 0 ? children : null;
       }
     }
   });
 
-  md.renderer.rules[kTokCite] = renderCite
-}
-
+  md.renderer.rules[kTokCite] = renderCite;
+};
 
 // Render pandoc-style divs
-function renderCite(tokens: Token[], idx: number, _options: MarkdownIt.Options, _env: unknown, self: Renderer): string {
-  const token = tokens[idx]; 
-  const citeContent =  `<code ${self.renderAttrs(token)}>${token.content}</code>`;
+function renderCite(
+  tokens: Token[],
+  idx: number,
+  _options: MarkdownIt.Options,
+  _env: unknown,
+  self: Renderer
+): string {
+  const token = tokens[idx];
+  const citeContent = `<code ${self.renderAttrs(token)}>${
+    token.content
+  }</code>`;
   return citeContent;
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/decorator.ts` & `jupyterlab_quarto-0.2.2/src/plugins/decorator.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,65 @@
 /*
-* fence.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
-import type MarkdownIt from "markdown-it/lib"
-import Token from "markdown-it/lib/token"
-import { attributeDecorator, decorator, DecoratorOptions } from "./utils/html";
-import { kTokDivOpen } from "./divs";
-import { kTokFigureOpen } from "./figures";
-import { kTokHeadingOpen, kTokTableOpen } from "./utils/tok";
-import { kTokMathBlock } from "./math";
-
-
-const kTokDecorator = "quarto_decorator";
-const kQuartoDecoratorOptions = "quarto-decorator-options";
+ * fence.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
+import type MarkdownIt from 'markdown-it/lib';
+import Token from 'markdown-it/lib/token';
+import { attributeDecorator, decorator, DecoratorOptions } from './utils/html';
+import { kTokDivOpen } from './divs';
+import { kTokFigureOpen } from './figures';
+import { kTokHeadingOpen, kTokTableOpen } from './utils/tok';
+import { kTokMathBlock } from './math';
 
+const kTokDecorator = 'quarto_decorator';
+const kQuartoDecoratorOptions = 'quarto-decorator-options';
 
 export const decoratorPlugin = (md: MarkdownIt) => {
-
-  md.core.ruler.push('quarto-decorator', function replaceAtSymbol(state) {
+  md.core.ruler.push('quarto-decorator', state => {
     const outTokens: Token[] = [];
     for (const token of state.tokens) {
-      if (token.type === "fence" && !token.attrs && token.info) {
+      if (token.type === 'fence' && !token.attrs && token.info) {
         outTokens.push(decoratorTokForToken(token));
       } else if (token.type === kTokHeadingOpen && token.attrs) {
         outTokens.push(decoratorTokForToken(token));
       } else if (token.type === kTokDivOpen && token.attrs) {
         outTokens.push(decoratorTokForToken(token));
       } else if (token.type === kTokFigureOpen && token.attrs) {
-        outTokens.push(decoratorTokForToken(token, { hide: { attributes: true }}));
+        outTokens.push(
+          decoratorTokForToken(token, { hide: { attributes: true } })
+        );
       } else if (token.type === kTokTableOpen && token.attrs) {
         outTokens.push(decoratorTokForToken(token));
       } else if (token.type === kTokMathBlock && token.attrs) {
         outTokens.push(decoratorTokForToken(token));
       }
       outTokens.push(token);
-    } 
+    }
     state.tokens = outTokens;
   });
-  
-  md.renderer.rules[kTokDecorator] = renderDecorator
-}
+
+  md.renderer.rules[kTokDecorator] = renderDecorator;
+};
 
 function decoratorTokForToken(token: Token, options?: DecoratorOptions) {
-  const decoratorTok = new Token(kTokDecorator, "div", 1);
+  const decoratorTok = new Token(kTokDecorator, 'div', 1);
   decoratorTok.attrs = token.attrs;
   decoratorTok.info = token.info;
   if (options) {
     decoratorTok.meta = decoratorTok.meta || {};
-    decoratorTok.meta[kQuartoDecoratorOptions] = options;  
+    decoratorTok.meta[kQuartoDecoratorOptions] = options;
   }
   return decoratorTok;
 }
 
-
 // Render pandoc-style divs
 function renderDecorator(tokens: Token[], idx: number): string {
   const token = tokens[idx];
   const decoratorOptions = token.meta?.[kQuartoDecoratorOptions];
   if (token.info) {
-    return decorator([token.info]) ;
+    return decorator([token.info]);
   } else {
     return attributeDecorator(token, decoratorOptions);
   }
 }
-
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/divs.ts` & `jupyterlab_quarto-0.2.2/src/plugins/divs.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,77 @@
 /*
-* divs.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
-import type MarkdownIt from "markdown-it/lib"
-import Token from "markdown-it/lib/token"
-import Renderer from "markdown-it/lib/renderer";
-import { addClass } from "./utils/markdownit";
+ * divs.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
+import type MarkdownIt from 'markdown-it/lib';
+import Token from 'markdown-it/lib/token';
+import Renderer from 'markdown-it/lib/renderer';
+import { addClass } from './utils/markdownit';
 
-export const kDivRuleName = "pandocDiv";
+export const kDivRuleName = 'pandocDiv';
 
 export const kTokDivOpen = 'pandoc_div_open';
 export const kTokDivClose = 'pandoc_div_close';
 
 export const divPlugin = (md: MarkdownIt) => {
-  
   // Render pandoc-style divs
-  function renderStartDiv(tokens: Token[], idx: number, _options: MarkdownIt.Options, _env: unknown, self: Renderer): string {
-
+  function renderStartDiv(
+    tokens: Token[],
+    idx: number,
+    _options: MarkdownIt.Options,
+    _env: unknown,
+    self: Renderer
+  ): string {
     // Add a class to designate that this is a quarto dev
     const token = tokens[idx];
-    token.attrs = addClass("quarto-div", token.attrs)
+    token.attrs = addClass('quarto-div', token.attrs);
 
     return `<div ${self.renderAttrs(token)}>`;
   }
 
   // Render pandoc-style divs
   function renderEndDiv(): string {
-    return `</div>`;
+    return '</div>';
   }
 
   // TODO Implement a better test during validation run
   // Handle pandoc-style divs
   md.block.ruler.before(
-    "fence",
+    'fence',
     kDivRuleName,
     (state, start, _end, silent) => {
-
       // This is a validation run, can ignore
       if (silent) {
         return true;
       }
-      
+
       // Get the line for parsing
       const lineStart = state.bMarks[start] + state.tShift[start];
       const lineEnd = state.eMarks[start];
-      const line = state.src.slice(lineStart, lineEnd)
-      
+      const line = state.src.slice(lineStart, lineEnd);
+
       // The current state of the divs (e.g. is there an open)
       // div. Data structure holds key that is the number of colons
       const divState = state.env.quartoOpenDivs || {};
 
       const incrementDivCount = (fence: string) => {
+        state.env.quartoDivLevel = (state.env.quartoDivLevel ?? 0) + 1;
         state.env.quartoOpenDivs = state.env.quartoOpenDivs || {};
         const current = state.env.quartoOpenDivs[fence] || 0;
         state.env.quartoOpenDivs[fence] = Math.max(0, current + 1);
-      }
+      };
 
       const decrementDivCount = (fence: string) => {
+        state.env.quartoDivLevel--;
         state.env.quartoOpenDivs = state.env.quartoOpenDivs || {};
         const current = state.env.quartoOpenDivs[fence] || 0;
         state.env.quartoOpenDivs[fence] = Math.max(0, current - 1);
-      }
+      };
 
       // Three or more colons followed by a an optional brace with attributes
       const divBraceRegex = /^(:::+)\s*(?:(\{[\s\S]+?\}))?$/;
 
       // Three or more colons followed by a string with no braces
       const divNoBraceRegex = /^(:::+)\s*(?:([^{}\s]+?))?$/;
 
@@ -93,42 +98,50 @@
           isOpenDiv = true;
         } else if (attr) {
           // If it has attributes it is always open
           isOpenDiv = true;
         }
 
         if (isOpenDiv) {
-          
           // Add to the open count (or set it to 1)
           incrementDivCount(divFence);
 
           // Make an open token
-          const token = state.push(kTokDivOpen, "div", 1)
+          const token = state.push(kTokDivOpen, 'div', 1);
           token.markup = line;
           // Allow this to be parsed for attributes by markdown-it-attr
-          if (attr && attr.startsWith("{")) {
+          if (attr && attr.startsWith('{')) {
             token.info = attr;
           } else if (attr) {
             token.info = `{.${attr}}`;
           }
           token.block = true;
+          token.meta = {
+            line: state.line,
+            level: state.env.quartoDivLevel
+          };
         } else {
           // Subtract from the open count (min zero)
+          const level = state.env.quartoDivLevel;
           decrementDivCount(divFence);
 
           // Make a close token
-          const token = state.push(kTokDivClose, "div", -1)
-          token.markup = line; 
+          const token = state.push(kTokDivClose, 'div', -1);
+          token.markup = line;
+          token.meta = {
+            line: state.line,
+            level
+          };
         }
 
-        state.line = start + 1
-        return true  
+        state.line = start + 1;
+        return true;
       } else {
         return false;
       }
     },
     { alt: [] }
-  )
+  );
 
-  md.renderer.rules[kTokDivOpen] = renderStartDiv
-  md.renderer.rules[kTokDivClose] = renderEndDiv
-}
+  md.renderer.rules[kTokDivOpen] = renderStartDiv;
+  md.renderer.rules[kTokDivClose] = renderEndDiv;
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/figure-divs.ts` & `jupyterlab_quarto-0.2.2/src/plugins/figure-divs.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 /*
  * figure-divs.ts
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
-import MarkdownIt from "markdown-it";
-import Token from "markdown-it/lib/token";
-import { readAttrValue } from "./utils/markdownit";
-import { kTokInline, kTokParaClose, kTokParaOpen } from "./utils/tok";
-import { kTokDivClose, kTokDivOpen } from "./divs";
-import { kTokFigCaptionClose, kTokFigCaptionOpen, mutateToFigureTok } from "./figures";
-
-
-const kFigureDivRuleName = "quarto-figure-divs";
-const kFigurePrefix = "fig-";
+import MarkdownIt from 'markdown-it';
+import Token from 'markdown-it/lib/token';
+import { readAttrValue } from './utils/markdownit';
+import { kTokInline, kTokParaClose, kTokParaOpen } from './utils/tok';
+import { kTokDivClose, kTokDivOpen } from './divs';
+import {
+  kTokFigCaptionClose,
+  kTokFigCaptionOpen,
+  mutateToFigureTok
+} from './figures';
 
+const kFigureDivRuleName = 'quarto-figure-divs';
+const kFigurePrefix = 'fig-';
 
 export const figureDivsPlugin = (md: MarkdownIt) => {
-  
   // Handle pandoc-style divs
-  md.core.ruler.push(
-    kFigureDivRuleName,
-    (state) => {
-
-      let isFigureDiv: boolean[] = [];
-
-      for (let i = 0; i < state.tokens.length; i++) {
-        const token = state.tokens[i];
-        if (token.type === kTokDivOpen) {
-          const id = readAttrValue("id", token.attrs);
-          if (id?.startsWith(kFigurePrefix)) {
-            isFigureDiv.push(true);  
-            mutateToFigureTok(token, "open");
-          } else {
-            // Note the div, but not a figure div
-            isFigureDiv.push(false);
-          }
-        } else if (token.type === kTokDivClose) {
-          const isFigDiv = isFigureDiv.pop();
-          if (isFigDiv) {
+  md.core.ruler.push(kFigureDivRuleName, state => {
+    const isFigureDiv: boolean[] = [];
 
-            // If the preview token is paragraph, use that as the caption
-            if (i - 3 >= 0) {
-              const maybeParaStart = state.tokens[i-3];
-              const maybeInline = state.tokens[i-2];
-              const maybeParaEnd = state.tokens[i-1];
-              if (maybeParaStart.type === kTokParaOpen && maybeParaEnd.type === kTokParaClose && maybeInline.type === kTokInline) {
-                mutateToFigCaption(state.tokens[i-3], "open");
-                mutateToFigCaption(state.tokens[i-1], "close");
-              }
+    for (let i = 0; i < state.tokens.length; i++) {
+      const token = state.tokens[i];
+      if (token.type === kTokDivOpen) {
+        const id = readAttrValue('id', token.attrs);
+        if (id?.startsWith(kFigurePrefix)) {
+          isFigureDiv.push(true);
+          mutateToFigureTok(token, 'open');
+        } else {
+          // Note the div, but not a figure div
+          isFigureDiv.push(false);
+        }
+      } else if (token.type === kTokDivClose) {
+        const isFigDiv = isFigureDiv.pop();
+        if (isFigDiv) {
+          // If the preview token is paragraph, use that as the caption
+          if (i - 3 >= 0) {
+            const maybeParaStart = state.tokens[i - 3];
+            const maybeInline = state.tokens[i - 2];
+            const maybeParaEnd = state.tokens[i - 1];
+            if (
+              maybeParaStart.type === kTokParaOpen &&
+              maybeParaEnd.type === kTokParaClose &&
+              maybeInline.type === kTokInline
+            ) {
+              mutateToFigCaption(state.tokens[i - 3], 'open');
+              mutateToFigCaption(state.tokens[i - 1], 'close');
             }
-            mutateToFigureTok(token, "close");
-          }  
+          }
+          mutateToFigureTok(token, 'close');
         }
       }
-    });
-  }
-
-  const mutateToFigCaption = (token: Token, type: "open" | "close") => {
-    token.tag = "figcaption";
-    token.type = type === "open" ? kTokFigCaptionClose : kTokFigCaptionOpen;
-  }
-
+    }
+  });
+};
+
+const mutateToFigCaption = (token: Token, type: 'open' | 'close') => {
+  token.tag = 'figcaption';
+  token.type = type === 'open' ? kTokFigCaptionClose : kTokFigCaptionOpen;
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/figures.ts` & `jupyterlab_quarto-0.2.2/src/plugins/figures.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,141 +1,139 @@
 /*
  * figures.ts
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
-import MarkdownIt from "markdown-it";
-import Token from "markdown-it/lib/token";
-import { kTokParaClose, kTokParaOpen } from "./utils/tok";
+import MarkdownIt from 'markdown-it';
+import Token from 'markdown-it/lib/token';
+import { kTokParaClose, kTokParaOpen } from './utils/tok';
 
 export interface FigureOptions {
   dataType?: boolean;
   link?: boolean;
   figcaption?: boolean;
   copyAttrs?: boolean;
   tabindex?: boolean;
   lazyLoading?: boolean;
 }
 
-export const kTokFigureOpen = "figure_open";
-export const kTokFigureClose = "figure_close";
+export const kTokFigureOpen = 'figure_open';
+export const kTokFigureClose = 'figure_close';
 
-export const kTokFigCaptionOpen = "figcaption_open";
-export const kTokFigCaptionClose = "figcaption_close";
+export const kTokFigCaptionOpen = 'figcaption_open';
+export const kTokFigCaptionClose = 'figcaption_close';
 
-export const mutateToFigureTok = (token: Token, type: "open" | "close") => {
-  token.type = type === "open" ? kTokFigureOpen : kTokFigureClose;
-  token.tag = "figure";
-}
+export const mutateToFigureTok = (token: Token, type: 'open' | 'close') => {
+  token.type = type === 'open' ? kTokFigureOpen : kTokFigureClose;
+  token.tag = 'figure';
+};
 
 export function figuresPlugin(md: MarkdownIt, options: FigureOptions) {
   options = options || {};
 
-  md.core.ruler.before("linkify", "implicit_figures", (state) => {
+  md.core.ruler.before('linkify', 'implicit_figures', state => {
     // reset tabIndex on md.render()
     let tabIndex = 1;
 
     // do not process first and last token
     for (let i = 1, l = state.tokens.length; i < l - 1; ++i) {
       const token = state.tokens[i];
 
-      if (token.type !== "inline") {
+      if (token.type !== 'inline') {
         continue;
       }
 
       // children: image alone, or link_open -> image -> link_close
       if (
         !token.children ||
         (token.children.length !== 1 && token.children.length !== 3)
       ) {
         continue;
       }
-      
+
       // one child, should be img
-      if (token.children.length === 1 && token.children[0].type !== "image") {
+      if (token.children.length === 1 && token.children[0].type !== 'image') {
         continue;
       }
 
       // three children, should be image enclosed in link
       if (
         token.children.length === 3 &&
-        (token.children[0].type !== "link_open" ||
-          token.children[1].type !== "image" ||
-          token.children[2].type !== "link_close")
+        (token.children[0].type !== 'link_open' ||
+          token.children[1].type !== 'image' ||
+          token.children[2].type !== 'link_close')
       ) {
         continue;
       }
 
-
       // prev token is paragraph open
       if (i !== 0 && state.tokens[i - 1].type !== kTokParaOpen) {
         continue;
       }
       // next token is paragraph close
       if (i !== l - 1 && state.tokens[i + 1].type !== kTokParaClose) {
         continue;
       }
 
       // The image
-      const image = token.children.length === 1 ? token.children[0] : token.children[1];
-      
+      const image =
+        token.children.length === 1 ? token.children[0] : token.children[1];
+
       // The image must have a caption to count as a figure
       if (!image.children || image.children.length === 0) {
         continue;
       }
-    
+
       // We have inline token containing an image only.
       // Previous token is paragraph open.
       // Next token is paragraph close.
       // Lets replace the paragraph tokens with figure tokens.
       const figure = state.tokens[i - 1];
-      mutateToFigureTok(figure, "open");
-      mutateToFigureTok(state.tokens[i + 1], "close");
+      mutateToFigureTok(figure, 'open');
+      mutateToFigureTok(state.tokens[i + 1], 'close');
 
-      if (options.dataType == true) {
-        state.tokens[i - 1].attrPush(["data-type", "image"]);
+      if (options.dataType === true) {
+        state.tokens[i - 1].attrPush(['data-type', 'image']);
       }
 
-      if (options.link == true && token.children.length === 1) {
-        token.children.unshift(new state.Token("link_open", "a", 1));
-        const src = image.attrGet("src");
+      if (options.link === true && token.children.length === 1) {
+        token.children.unshift(new state.Token('link_open', 'a', 1));
+        const src = image.attrGet('src');
         if (src !== null) {
-          token.children[0].attrPush(["href", src]);
+          token.children[0].attrPush(['href', src]);
         }
-        token.children.push(new state.Token("link_close", "a", -1));
+        token.children.push(new state.Token('link_close', 'a', -1));
       }
 
-
-
-      if (options.figcaption == true) {
+      if (options.figcaption === true) {
         if (image.children && image.children.length) {
           token.children.push(
-            new state.Token(kTokFigCaptionOpen, "figcaption", 1)
+            new state.Token(kTokFigCaptionOpen, 'figcaption', 1)
           );
           token.children.splice(token.children.length, 0, ...image.children);
           token.children.push(
-            new state.Token(kTokFigCaptionClose, "figcaption", -1)
+            new state.Token(kTokFigCaptionClose, 'figcaption', -1)
           );
           image.children.length = 0;
         }
       }
 
       if (options.copyAttrs && image.attrs) {
-        const f = options.copyAttrs === true ? "" : options.copyAttrs;
+        const f = options.copyAttrs === true ? '' : options.copyAttrs;
         figure.attrs = image.attrs.filter(([k]) => k.match(f));
       }
 
-      if (options.tabindex == true) {
+      if (options.tabindex === true) {
         // add a tabindex property
         // you could use this with css-tricks.com/expanding-images-html5
-        state.tokens[i - 1].attrPush(["tabindex", String(tabIndex)]);
+        state.tokens[i - 1].attrPush(['tabindex', String(tabIndex)]);
         tabIndex++;
       }
 
-      if (options.lazyLoading == true) {
-        image.attrPush(["loading", "lazy"]);
+      if (options.lazyLoading === true) {
+        image.attrPush(['loading', 'lazy']);
       }
     }
   });
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/math.ts` & `jupyterlab_quarto-0.2.2/src/plugins/math.ts`

 * *Files 12% similar despite different names*

```diff
@@ -10,26 +10,25 @@
 /*
 Like markdown-it-simplemath, this is a stripped down, simplified version of:
 https://github.com/runarberg/markdown-it-math
 
 It differs in that it takes (a subset of) LaTeX as input and relies on MathJax
 for rendering output.
 */
-import type MarkdownIt from "markdown-it";
+import type MarkdownIt from 'markdown-it';
 
-import type Token from "markdown-it/lib/token";
-import type StateInline from "markdown-it/lib/rules_inline/state_inline";
-import type StateBlock from "markdown-it/lib/rules_block/state_block";
-
-export const kTokMathBlock = "math_block";
-export const kTokMathInline = "math_inline";
+import type Token from 'markdown-it/lib/token';
+import type StateInline from 'markdown-it/lib/rules_inline/state_inline';
+import type StateBlock from 'markdown-it/lib/rules_block/state_block';
 
+export const kTokMathBlock = 'math_block';
+export const kTokMathInline = 'math_inline';
 
 interface ConvertOptions {
-  display: boolean
+  display: boolean;
 }
 
 function renderMath(content: string, convertOptions: ConvertOptions): string {
   if (convertOptions.display) {
     return `<div class='quarto-display-math'>\\[${content}\\]</div>`;
   } else {
     return `<span class='quarto-inline-math'>\\(${content}\\)</span>`;
@@ -57,84 +56,84 @@
   }
   if (nextChar === 0x20 /* " " */ || nextChar === 0x09 /* \t */) {
     can_open = false;
   }
 
   return {
     can_open: can_open,
-    can_close: can_close,
+    can_close: can_close
   };
 }
 
 function math_inline(state: StateInline, silent: boolean) {
-  if (state.src[state.pos] !== "$") {
+  if (state.src[state.pos] !== '$') {
     return false;
   }
 
   let res = isValidDelim(state, state.pos);
   if (!res.can_open) {
     if (!silent) {
-      state.pending += "$";
+      state.pending += '$';
     }
     state.pos += 1;
     return true;
   }
 
   // First check for and bypass all properly escaped delimieters
   // This loop will assume that the first leading backtick can not
   // be the first character in state.src, which is known since
   // we have found an opening delimieter already.
   const start = state.pos + 1;
   let match = start;
-  while ((match = state.src.indexOf("$", match)) !== -1) {
+  while ((match = state.src.indexOf('$', match)) !== -1) {
     // Found potential $, look for escapes, pos will point to
     // first non escape when complete
     let pos = match - 1;
-    while (state.src[pos] === "\\") {
+    while (state.src[pos] === '\\') {
       pos -= 1;
     }
 
     // Even number of escapes, potential closing delimiter found
-    if ((match - pos) % 2 == 1) {
+    if ((match - pos) % 2 === 1) {
       break;
     }
     match += 1;
   }
 
   // No closing delimter found.  Consume $ and continue.
   if (match === -1) {
     if (!silent) {
-      state.pending += "$";
+      state.pending += '$';
     }
     state.pos = start;
     return true;
   }
 
   // Check if we have empty content, ie: $$.  Do not parse.
   if (match - start === 0) {
     if (!silent) {
-      state.pending += "$$";
+      state.pending += '$$';
     }
     state.pos = start + 1;
     return true;
   }
 
   // Check for valid closing delimiter
   res = isValidDelim(state, match);
   if (!res.can_close) {
     if (!silent) {
-      state.pending += "$";
+      state.pending += '$';
     }
     state.pos = start;
     return true;
   }
 
   if (!silent) {
-    const token = state.push("math_inline", "math", 0);
-    token.markup = "$";
+    const token = state.push('math_inline', 'math', 0);
+    token.markup = '$';
     token.content = state.src.slice(start, match);
   }
 
   state.pos = match + 1;
   return true;
 }
 
@@ -144,30 +143,30 @@
   end: number,
   silent: boolean
 ) {
   let next: number, lastPos: number;
   let found = false,
     pos = state.bMarks[start] + state.tShift[start],
     max = state.eMarks[start],
-    lastLine = "";
+    lastLine = '';
 
   if (pos + 2 > max) {
     return false;
   }
-  if (state.src.slice(pos, pos + 2) !== "$$") {
+  if (state.src.slice(pos, pos + 2) !== '$$') {
     return false;
   }
 
   pos += 2;
   let firstLine = state.src.slice(pos, max);
 
   if (silent) {
     return true;
   }
-  if (firstLine.trim().slice(-2) === "$$") {
+  if (firstLine.trim().slice(-2) === '$$') {
     // Single line expression
     firstLine = firstLine.trim().slice(0, -2);
     found = true;
   }
 
   let attrStr = undefined;
   for (next = start; !found; ) {
@@ -184,51 +183,59 @@
       // non-empty line with negative indent should stop the list:
       break;
     }
 
     const line = state.src.slice(pos, max).trim();
     const match = line.match(/^\$\$\s*(\{.*\})?\s*$/);
     if (match) {
-      lastPos = state.src.slice(0, max).lastIndexOf("$$");
+      lastPos = state.src.slice(0, max).lastIndexOf('$$');
       lastLine = state.src.slice(pos, lastPos);
       attrStr = match[1];
       found = true;
     }
   }
 
   state.line = next + 1;
 
-  const token = state.push(kTokMathBlock, "math", 0);
+  const token = state.push(kTokMathBlock, 'math', 0);
   token.block = true;
   if (attrStr) {
     token.info = attrStr;
   }
   token.content =
-    (firstLine && firstLine.trim() ? firstLine + "\n" : "") +
+    (firstLine && firstLine.trim() ? firstLine + '\n' : '') +
     state.getLines(start + 1, next, state.tShift[start], true) +
-    (lastLine && lastLine.trim() ? lastLine : "");
+    (lastLine && lastLine.trim() ? lastLine : '');
   token.map = [start, state.line];
-  token.markup = "$$";
+  token.markup = '$$';
   return true;
 }
 
-export function mathjaxPlugin(md: MarkdownIt) {
+export function mathjaxPlugin(
+  md: MarkdownIt,
+  options?: { enableInlines?: boolean }
+) {
   // Default options
+  options = options || {};
+  const enableInlines =
+    options.enableInlines !== undefined ? options.enableInlines : true;
 
   const convertOptions = {
     display: false
-  }
+  };
 
   // set MathJax as the renderer for markdown-it-simplemath
-  md.inline.ruler.after("escape", kTokMathInline, math_inline);
-  md.block.ruler.after("blockquote", kTokMathBlock, math_block, {
-    alt: ["paragraph", "reference", "blockquote", "list"],
+  md.inline.ruler.after('escape', kTokMathInline, math_inline);
+  md.block.ruler.after('blockquote', kTokMathBlock, math_block, {
+    alt: ['paragraph', 'reference', 'blockquote', 'list']
   });
-  md.renderer.rules.math_inline = function (tokens: Token[], idx: number) {
-    convertOptions.display = false;
-    return renderMath(tokens[idx].content, convertOptions)
-  };
+  if (enableInlines) {
+    md.renderer.rules.math_inline = function (tokens: Token[], idx: number) {
+      convertOptions.display = false;
+      return renderMath(tokens[idx].content, convertOptions);
+    };
+  }
   md.renderer.rules.math_block = function (tokens: Token[], idx: number) {
     convertOptions.display = true;
-    return renderMath(tokens[idx].content, convertOptions)
+    return renderMath(tokens[idx].content, convertOptions);
   };
-};
+}
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/shortcodes.ts` & `jupyterlab_quarto-0.2.2/src/plugins/shortcodes.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 /*
-* shortcodes.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
-import type MarkdownIt from "markdown-it/lib"
-import Token from "markdown-it/lib/token"
+ * shortcodes.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
+import type MarkdownIt from 'markdown-it/lib';
+import Token from 'markdown-it/lib/token';
 
-import StateInline from "markdown-it/lib/rules_inline/state_inline";
-import { escapeHtml } from "markdown-it/lib/common/utils";
+import StateInline from 'markdown-it/lib/rules_inline/state_inline';
+import { escapeHtml } from 'markdown-it/lib/common/utils';
 
-export const kShortcode = "shortcode";
+export const kShortcode = 'shortcode';
 
 export const shortcodePlugin = (md: MarkdownIt) => {
   const shortcode = (state: StateInline, silent: boolean): boolean => {
     // {{< shortcode >}}
-    if (state.src.slice(state.pos, state.pos + 3) !== "{{<") {
+    if (state.src.slice(state.pos, state.pos + 3) !== '{{<') {
       return false;
     }
     const shortcodeEndRegex = />}}/g;
 
     // ignore if shortcode doesn't end
     const end = state.src.slice(state.pos).search(shortcodeEndRegex);
     if (end === -1) {
       return false;
     }
 
     const shortcodeContent = state.src.slice(state.pos + 3, state.pos + end);
     if (!silent) {
-      const token = state.push("shortcode", "shortcode", 0);
-      token.markup = "";
+      const token = state.push('shortcode', 'shortcode', 0);
+      token.markup = '';
       token.content = shortcodeContent;
     }
     state.pos += end + 3;
     return true;
-  }
-  md.inline.ruler.after("escape", kShortcode, shortcode);
+  };
+  md.inline.ruler.after('escape', kShortcode, shortcode);
 
   const renderShortcode = (tokens: Token[], idx: number): string => {
     const token = tokens[idx];
     const content = token.content;
     // insert shortcode braces and escape content's html entities
     return `<span class="shortcode">${escapeHtml(`{{<${content}>}}`)}</span>`;
-  }
+  };
 
   md.renderer.rules[kShortcode] = renderShortcode;
-}
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/spans.ts` & `jupyterlab_quarto-0.2.2/src/plugins/spans.ts`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 /*
  * span.ts
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
-import MarkdownIt from "markdown-it";
-import StateInline from "markdown-it/lib/rules_inline/state_inline";
-
+import MarkdownIt from 'markdown-it';
+import StateInline from 'markdown-it/lib/rules_inline/state_inline';
 
 export function spansPlugin(md: MarkdownIt) {
   function span(state: StateInline) {
-    const max = state.posMax
+    const max = state.posMax;
 
-    if (state.src.charCodeAt(state.pos) !== 0x5B) {
+    if (state.src.charCodeAt(state.pos) !== 0x5b) {
       // opening [
       return false;
     }
 
     const labelStart = state.pos + 1;
-    const labelEnd   = state.md.helpers.parseLinkLabel(state, state.pos, true);
+    const labelEnd = state.md.helpers.parseLinkLabel(state, state.pos, true);
 
     if (labelEnd < 0) {
       // parser failed to find closing ]
       return false;
     }
 
     const pos = labelEnd + 1;
-    if (pos < max && state.src.charCodeAt(pos) === 0x7B /* { */) {
+    if (pos < max && state.src.charCodeAt(pos) === 0x7b /* { */) {
       // probably found span
 
       state.pos = labelStart;
       state.posMax = labelEnd;
 
       state.push('span_open', 'span', 1);
       state.md.inline.tokenize(state);
@@ -39,10 +38,10 @@
 
       state.pos = pos;
       state.posMax = max;
       return true;
     } else {
       return false;
     }
-  };
+  }
   md.inline.ruler.push('quarto-spans', span);
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/table-captions.ts` & `jupyterlab_quarto-0.2.2/src/plugins/table-captions.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,105 @@
 /*
  * table-captions.ts
  *
  * Copyright (C) 2020-2023 Posit Software, PBC
  *
  */
 
-import MarkdownIt from "markdown-it";
-import Token from "markdown-it/lib/token";
-import { kTokInline, kTokParaClose, kTokParaOpen, kTokTableClose, kTokTableOpen, kTokText } from "./utils/tok";
+import MarkdownIt from 'markdown-it';
+import Token from 'markdown-it/lib/token';
+import {
+  kTokInline,
+  kTokParaClose,
+  kTokParaOpen,
+  kTokTableClose,
+  kTokTableOpen,
+  kTokText
+} from './utils/tok';
 
-
-const kTableCaptionRule = "quarto-table-captions";
+const kTableCaptionRule = 'quarto-table-captions';
 
 export const tableCaptionPlugin = (md: MarkdownIt) => {
-  
-  md.core.ruler.push(
-    kTableCaptionRule,
-    (state) => {
-
-      const tableIdxs: number[] = [];
-      const tablePoss: TablePos[] = [];
-  
-      // Identify tables that we'd like to process
-      // The tables must be the bottom first (we will process them bottom to
-      // top to ensure that the positions remain accurate as the tokens
-      // are mutated
-      for (let i = 0; i < state.tokens.length; i++) {
-        const token = state.tokens[i];
-        if (token.type === kTokTableOpen) {
-          tableIdxs.push(i);
-        } else if (token.type === kTokTableClose) {          
-          const start = tableIdxs.pop();
-          if (start) {
-            tablePoss.unshift({
-              start,
-              end: i
-            })
-          }
+  md.core.ruler.push(kTableCaptionRule, state => {
+    const tableIdxs: number[] = [];
+    const tablePoss: TablePos[] = [];
+
+    // Identify tables that we'd like to process
+    // The tables must be the bottom first (we will process them bottom to
+    // top to ensure that the positions remain accurate as the tokens
+    // are mutated
+    for (let i = 0; i < state.tokens.length; i++) {
+      const token = state.tokens[i];
+      if (token.type === kTokTableOpen) {
+        tableIdxs.push(i);
+      } else if (token.type === kTokTableClose) {
+        const start = tableIdxs.pop();
+        if (start) {
+          tablePoss.unshift({
+            start,
+            end: i
+          });
         }
       }
+    }
 
-      // Look just past the tables and if there is a paragraph that is 
-      // a table caption, extract that and place it in the table      
-      for (const tablePos of tablePoss) {
-        resolveTableCaption(state.tokens, tablePos.start, tablePos.end);
-      }
-    });
-  }
+    // Look just past the tables and if there is a paragraph that is
+    // a table caption, extract that and place it in the table
+    for (const tablePos of tablePoss) {
+      resolveTableCaption(state.tokens, tablePos.start, tablePos.end);
+    }
+  });
+};
+
+function resolveTableCaption(
+  tokens: Token[],
+  tblStartPos: number,
+  tblEndPos: number
+) {
+  // Must have at least three tokens past the table end
+  if (tokens.length > tblEndPos + 3) {
+    if (
+      tokens[tblEndPos + 1].type === kTokParaOpen &&
+      tokens[tblEndPos + 2].type === kTokInline &&
+      tokens[tblEndPos + 3].type === kTokParaClose
+    ) {
+      const maybeCaption = tokens[tblEndPos + 2];
+
+      const isText =
+        maybeCaption.children !== null &&
+        maybeCaption.children.length > 0 &&
+        maybeCaption.children[0].type === kTokText;
+      const maybeCaptionText =
+        isText && maybeCaption.children ? maybeCaption.children[0].content : '';
+      const match = maybeCaptionText.match(/^:\s([^{}]*)(?:\{.*\}){0,1}$/);
+      if (match && match[1]) {
+        // Carve out the existing tokens
+        const capTokens = tokens.splice(tblEndPos + 1, 3);
+
+        // We have the caption, remove the paragraph and return
+        // the caption
+        capTokens[0].type = 'table_caption';
+        capTokens[0].tag = 'caption';
+
+        // Forward any attributes from the caption up to the table
+        tokens[tblStartPos].attrs = capTokens[0].attrs;
+        capTokens[0].attrs = [];
+
+        // Trim the content
+        if (capTokens[1].children && capTokens[1].children.length > 0) {
+          capTokens[1].children[0].content = match[1];
+        }
 
+        // Close the caption
+        capTokens[2].type = 'table_caption';
+        capTokens[2].tag = 'caption';
 
-  function resolveTableCaption(tokens: Token[], tblStartPos: number, tblEndPos: number) {
-    // Must have at least three tokens past the table end
-    if (tokens.length > tblEndPos + 3) {
-      if (tokens[tblEndPos + 1].type === kTokParaOpen 
-        && tokens[tblEndPos + 2].type === kTokInline
-        && tokens[tblEndPos + 3].type === kTokParaClose) {
-
-          const maybeCaption = tokens[tblEndPos + 2];
-          
-          const isText = maybeCaption.children !== null && maybeCaption.children.length > 0 && maybeCaption.children[0].type === kTokText;
-          const maybeCaptionText = isText ? maybeCaption.children![0].content : "";
-          const match = maybeCaptionText.match(/^:\s([^{}]*)(?:\{.*\}){0,1}$/);
-          if (match && match[1]) {
-
-            // Carve out the existing tokens
-            const capTokens = tokens.splice(tblEndPos + 1, 3);
-
-            // We have the caption, remove the paragraph and return
-            // the caption
-            capTokens[0].type = "table_caption";
-            capTokens[0].tag = "caption";
-
-            // Forward any attributes from the caption up to the table
-            tokens[tblStartPos].attrs = capTokens[0].attrs;
-            capTokens[0].attrs = [];
-
-            // Trim the content
-            capTokens[1].children![0].content = match[1];
-
-            // Close the caption
-            capTokens[2].type = "table_caption";
-            capTokens[2].tag = "caption";
-
-            tokens.splice(tblStartPos + 1, 0, ...capTokens);
-          } 
-      } 
-    } 
+        tokens.splice(tblStartPos + 1, 0, ...capTokens);
+      }
+    }
   }
+}
 
-  interface TablePos {
-    start: number,
-    end: number
-  }
+interface TablePos {
+  start: number;
+  end: number;
+}
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/yaml.ts` & `jupyterlab_quarto-0.2.2/src/plugins/yaml.ts`

 * *Files 13% similar despite different names*

```diff
@@ -10,28 +10,28 @@
  * GNU Affero General Public License. This program is distributed WITHOUT
  * ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING THOSE OF NON-INFRINGEMENT,
  * MERCHANTABILITY OR FITNESS FOR A PARTICULAR PURPOSE. Please refer to the
  * AGPL (http://www.gnu.org/licenses/agpl-3.0.txt) for more details.
  *
  */
 
-import MarkdownIt from "markdown-it";
-import StateBlock from "markdown-it/lib/rules_block/state_block";
-import Token from "markdown-it/lib/token";
-import * as yaml from "js-yaml";
-import { decorator } from "./utils/html";
+import MarkdownIt from 'markdown-it';
+import StateBlock from 'markdown-it/lib/rules_block/state_block';
+import Token from 'markdown-it/lib/token';
+import * as yaml from 'js-yaml';
+import { decorator } from './utils/html';
 
 // Typescript version of https://github.com/parksb/markdown-it-front-matter
 // TODO: Rationalize this with quarto-core/src/markdownit-yaml.ts
 //       This is a copy with rendering added - the core tokenizing function is identical (or should be)
 const kTokFrontMatter = 'front_matter';
 
 export function yamlPlugin(md: MarkdownIt, cb?: (yaml: unknown) => void) {
   const min_markers = 3,
-    marker_str = "-",
+    marker_str = '-',
     marker_char = marker_str.charCodeAt(0),
     marker_len = marker_str.length;
 
   function frontMatter(
     state: StateBlock,
     startLine: number,
     endLine: number,
@@ -77,15 +77,15 @@
       nextLine++;
       if (nextLine >= endLine) {
         // unclosed block should be autoclosed by end of document.
         // also block seems to be autoclosed by end of parent
         break;
       }
 
-      if (state.src.slice(start, max) === "...") {
+      if (state.src.slice(start, max) === '...') {
         break;
       }
 
       start = state.bMarks[nextLine] + state.tShift[nextLine];
       max = state.eMarks[nextLine];
 
       if (start < max && state.sCount[nextLine] < state.blkIndent) {
@@ -127,109 +127,107 @@
       user_closed = true;
       break;
     }
 
     // Ensure that we have real yaml here
     const markup = state.src.slice(startLine, pos);
     const yaml = parseFrontMatterStr(markup);
-    const isYamlBlock = yaml !== null && typeof(yaml) === "object";
-    
+    const isYamlBlock = yaml !== null && typeof yaml === 'object';
+
     // If this is yaml, render it
     if (isYamlBlock && user_closed) {
       const old_parent = state.parentType;
       const old_line_max = state.lineMax;
-  
-      const token = state.push(kTokFrontMatter, "", 0);
+
+      const token = state.push(kTokFrontMatter, '', 0);
       token.hidden = true;
       token.markup = markup;
       token.block = true;
       token.map = [startLine, pos];
       token.meta = state.src.slice(start_content, start - 1);
-  
+
       if (cb) {
         cb(token.meta);
-      }    
+      }
       state.parentType = old_parent;
-      state.lineMax = old_line_max;  
+      state.lineMax = old_line_max;
       state.line = nextLine + (user_closed ? 1 : 0);
       return true;
     } else {
       // This is not yaml, just continue
       state.line = nextLine + 1;
       return false;
     }
   }
 
-  md.block.ruler.before("table", kTokFrontMatter, frontMatter, {
-    alt: ["paragraph", "reference", "blockquote", "list"],
+  md.block.ruler.before('table', kTokFrontMatter, frontMatter, {
+    alt: ['paragraph', 'reference', 'blockquote', 'list']
   });
 
   // Add rendering
-  md.renderer.rules[kTokFrontMatter] = renderFrontMatter
+  md.renderer.rules[kTokFrontMatter] = renderFrontMatter;
 }
 
 function renderFrontMatter(tokens: Token[], idx: number): string {
   const token = tokens[idx];
 
   // Parse the markup
   const frontUnknown = parseFrontMatterStr(token.markup);
 
   // Extract important content
-  if (typeof(frontUnknown) === "object") {
+  if (typeof frontUnknown === 'object') {
     const titleBlock: TitleBlock = {};
     const frontMatter = frontUnknown as Record<string, unknown>;
 
     const readStr = (key: string) => {
       if (frontMatter[key] === undefined) {
         return undefined;
-      } else if (typeof(frontMatter[key]) === "string") {
+      } else if (typeof frontMatter[key] === 'string') {
         const val = frontMatter[key] as string;
         delete frontMatter[key];
         return val;
       } else {
         return undefined;
       }
-    }
-    
+    };
+
     // Read simple values
-    titleBlock.title = readStr("title");
-    titleBlock.subtitle = readStr("subtitle");
-    titleBlock.abstract = readStr("abstract");
-    titleBlock.date = readStr("date");
-    titleBlock.modified = readStr("date-modified");
-    titleBlock.doi = readStr("doi");
-    
+    titleBlock.title = readStr('title');
+    titleBlock.subtitle = readStr('subtitle');
+    titleBlock.abstract = readStr('abstract');
+    titleBlock.date = readStr('date');
+    titleBlock.modified = readStr('date-modified');
+    titleBlock.doi = readStr('doi');
+
     // Read Authors
     titleBlock.authors = parseAuthor(frontMatter.author || frontMatter.authors);
     delete frontMatter.author;
     delete frontMatter.authors;
 
-
     // The final rendered HTML output
     const titleLines: string[] = [];
 
     // Render the title block and other yaml options
     const titleRendered = renderTitle(titleBlock);
     titleLines.push(titleRendered);
 
     if (Object.keys(frontMatter).length > 0) {
-
       // decorator
-      const decor = decorator(["Options"]);
+      const decor = decorator(['Options']);
       titleLines.push(decor);
 
       // yaml
       const yamlDump = yaml.dump(frontMatter);
       const otherYamlRendered = `<pre class="quarto-frontmatter-container"><code class="cm-s-jupyter language-yaml quarto-frontmatter">${yamlDump}</code></pre>`;
 
       titleLines.push(otherYamlRendered);
     }
-    return titleLines.join("\n");
+    return titleLines.join('\n');
   } else {
-    return "";
+    return '';
   }
 }
 
 interface Author {
   name: string;
   affil?: string[];
   orcid?: string;
@@ -238,27 +236,27 @@
 interface TitleBlock {
   title?: string;
   subtitle?: string;
   abstract?: string;
   date?: string;
   modified?: string;
   doi?: string;
-  authors?: Author[]; 
+  authors?: Author[];
 }
 
 type DocMetaValue = {
   value: string;
-  padded?: boolean
+  padded?: boolean;
 };
 
 // TODO: Use core function instead
 function parseFrontMatterStr(str: string) {
-  str = str.replace(/---\s*$/, "");
+  str = str.replace(/---\s*$/, '');
   try {
-    return yaml.load(str, { schema: yaml.FAILSAFE_SCHEMA});
+    return yaml.load(str, { schema: yaml.FAILSAFE_SCHEMA });
   } catch (error) {
     return undefined;
   }
 }
 
 function renderTitle(titleBlock: TitleBlock) {
   const rendered: string[] = [];
@@ -271,144 +269,153 @@
   }
 
   const metadataBlocks: string[] = [];
 
   if (titleBlock.authors && titleBlock.authors?.length > 0) {
     const names: DocMetaValue[] = [];
     const affils: DocMetaValue[] = [];
-    
 
     for (let i = 0; i < titleBlock.authors.length; i++) {
-      const author = titleBlock.authors[i];      
+      const author = titleBlock.authors[i];
       if (author.orcid) {
-        names.push(
-          { 
-            value: `${author.name}<a href="https://orcid.org/${author.orcid}" class="quarto-orcid"><i></i></a>`,
-            padded: i > 0
-          });
+        names.push({
+          value: `${author.name}<a href="https://orcid.org/${author.orcid}" class="quarto-orcid"><i></i></a>`,
+          padded: i > 0
+        });
       } else {
-        names.push({ value: author.name, padded: i > 0 })
+        names.push({ value: author.name, padded: i > 0 });
       }
-      
+
       // Place empty rows to allow affiliations to line up
-      const emptyCount = author.affil ? Math.max(author.affil.length - 1, 0) : 0;
+      const emptyCount = author.affil
+        ? Math.max(author.affil.length - 1, 0)
+        : 0;
       for (let j = 0; j < emptyCount; j++) {
-        names.push({ value: "&nbsp;"});
+        names.push({ value: '&nbsp;' });
       }
 
       // Collect affilations
       if (author.affil) {
         for (let k = 0; k < author.affil.length; k++) {
           const affil = author.affil[k];
           affils.push({
             value: affil,
-            padded: i > 0 && k == 0
+            padded: i > 0 && k === 0
           });
         }
-  
       }
     }
 
-    const authLabel = names.length === 1 ? "Author" : "Authors";
+    const authLabel = names.length === 1 ? 'Author' : 'Authors';
     metadataBlocks.push(renderDocMeta(authLabel, names));
 
     if (affils.length > 0) {
-      const affilLabel = affils.length === 1 ? "Affiliation" : "Affiliations";
+      const affilLabel = affils.length === 1 ? 'Affiliation' : 'Affiliations';
       metadataBlocks.push(renderDocMeta(affilLabel, affils));
     }
-
   }
-  
+
   if (titleBlock.date) {
-    metadataBlocks.push(renderDocMeta("Date", [{value: titleBlock.date}]));
+    metadataBlocks.push(renderDocMeta('Date', [{ value: titleBlock.date }]));
   }
-  
+
   if (titleBlock.modified) {
-    metadataBlocks.push(renderDocMeta("Modified", [{value: titleBlock.modified}]));
+    metadataBlocks.push(
+      renderDocMeta('Modified', [{ value: titleBlock.modified }])
+    );
   }
 
   if (titleBlock.doi) {
-    metadataBlocks.push(renderDocMeta("DOI", [{value: `<a href="https://doi.org/${titleBlock.doi}">${titleBlock.doi}</a>`}]));
+    metadataBlocks.push(
+      renderDocMeta('DOI', [
+        {
+          value: `<a href="https://doi.org/${titleBlock.doi}">${titleBlock.doi}</a>`
+        }
+      ])
+    );
   }
 
   if (metadataBlocks.length > 0) {
     rendered.push(renderDocMetas(metadataBlocks));
   }
 
   if (titleBlock.abstract) {
     rendered.push(`<p class="quarto-abstract">${titleBlock.abstract}</p>`);
   }
 
-  return rendered.join("\n");
+  return rendered.join('\n');
 }
 
 function renderDocMetas(docMetas: string[]) {
   const rendered: string[] = [];
 
-  rendered.push(`<div class="quarto-meta-block">`);
-  docMetas.forEach((docMeta) => { rendered.push(docMeta)});
-  rendered.push(`</div>`);
+  rendered.push('<div class="quarto-meta-block">');
+  docMetas.forEach(docMeta => {
+    rendered.push(docMeta);
+  });
+  rendered.push('</div>');
 
-  return rendered.join("\n");
+  return rendered.join('\n');
 }
 
 function renderDocMeta(label: string, vals: DocMetaValue[]) {
   const rendered: string[] = [];
 
-  rendered.push(`<div class="quarto-meta">`);
+  rendered.push('<div class="quarto-meta">');
   rendered.push(`<p class="quarto-meta-title">${label}</p>`);
-  vals.forEach((val) => {
-    const clz = val.padded ? ` class="quarto-meta-padded"` : "";
+  vals.forEach(val => {
+    const clz = val.padded ? ' class="quarto-meta-padded"' : '';
     rendered.push(`<p${clz}>${val.value}</p>`);
   });
-  rendered.push(`</div>`);
+  rendered.push('</div>');
 
-  return rendered.join("\n");
+  return rendered.join('\n');
 }
 
-function parseAuthor(author: unknown) : Author[] {
+function parseAuthor(author: unknown): Author[] {
   const authorsRaw = Array.isArray(author) ? author : [author];
   const authors: Author[] = [];
   for (const authorRaw of authorsRaw) {
-    if (typeof(authorRaw) === "string") {
+    if (typeof authorRaw === 'string') {
       authors.push({
         name: authorRaw
       });
-    } else if (typeof(authorRaw) === "object") {
-
+    } else if (typeof authorRaw === 'object') {
       const str = (key: string, defaultValue?: string) => {
-        if (typeof(authorRaw[key]) === "string") {
+        if (typeof authorRaw[key] === 'string') {
           return authorRaw[key] as string;
         } else {
           return defaultValue;
         }
-      }
+      };
 
       const affiliations: string[] = [];
-      const affiliationSimple = str("affiliation");
+      const affiliationSimple = str('affiliation');
       if (affiliationSimple) {
         affiliations.push(affiliationSimple);
       } else if (authorRaw.affiliations) {
-        const affils = Array.isArray(authorRaw.affiliations) ? authorRaw.affiliations as unknown[] : [authorRaw.affiliations];
+        const affils = Array.isArray(authorRaw.affiliations)
+          ? (authorRaw.affiliations as unknown[])
+          : [authorRaw.affiliations];
         affils.forEach((affilRaw: unknown) => {
-          if (typeof(affilRaw) === "string") {
+          if (typeof affilRaw === 'string') {
             affiliations.push(affilRaw);
-          // eslint-disable-next-line no-constant-condition
-          } else if (typeof(affilRaw === "object")) {
+            // eslint-disable-next-line no-constant-condition
+          } else if (typeof (affilRaw === 'object')) {
             const affilRecord = affilRaw as Record<string, unknown>;
             const name = affilRecord.name;
-            if (typeof(name) === "string") {
+            if (typeof name === 'string') {
               affiliations.push(name);
             }
           }
         });
       }
 
       authors.push({
-        name: str("name", "")!,
-        orcid: str("orcid"),
+        name: str('name', '') ?? '',
+        orcid: str('orcid'),
         affil: affiliations
-      })
+      });
     }
   }
   return authors;
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/gridtables/GetCells.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/gridtables/GetCells.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,55 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
 /**
-* getCells parses the lines found for a certain row, and transforms these to
-* the separate cell lines.
-* 
-* @param lines The lines for the row.
-*/
-export default function getCells(
-    lines: string[][]):
-    string[][]
-{
-    const cells = [];
-
-    for (let i = 0; i < lines[0].length; i++)
-    {
-        let cell = [];
-
-        for (let j = 0; j < lines.length; j++)
-        {
-            const s = trimEnd(lines[j][i]);
-
-            if ((s.length === 0) &&
-                (cell.length === 0))
-            {
-                // skip leading empty lines
-                continue;
-            }
-
-            cell.push(s);
-        }
-
-        // remove trailing empty lines
-        let j = cell.length - 1;
-        for (; j >= 0; j--)
-        {
-            if (cell[j].length > 0)
-            {
-                break;
-            }
-        }
-
-        if (j < cell.length - 1)
-        {
-            cell = cell.slice(0, j + 1);
-        }
+ * getCells parses the lines found for a certain row, and transforms these to
+ * the separate cell lines.
+ *
+ * @param lines The lines for the row.
+ */
+export default function getCells(lines: string[][]): string[][] {
+  const cells = [];
+
+  for (let i = 0; i < lines[0].length; i++) {
+    let cell = [];
+
+    for (let j = 0; j < lines.length; j++) {
+      const s = trimEnd(lines[j][i]);
+
+      if (s.length === 0 && cell.length === 0) {
+        // skip leading empty lines
+        continue;
+      }
 
-        cells.push(cell);
+      cell.push(s);
     }
 
-    return cells;
-}
+    // remove trailing empty lines
+    let j = cell.length - 1;
+    for (; j >= 0; j--) {
+      if (cell[j].length > 0) {
+        break;
+      }
+    }
 
-function trimEnd(
-    s: string):
-    string
-{
-    const trimmed = s.trim();
-
-    if (trimmed.length === 0)
-    {
-        return '';
+    if (j < cell.length - 1) {
+      cell = cell.slice(0, j + 1);
     }
 
-    return s.slice(
-        0,
-        s.indexOf(trimmed) + trimmed.length);
+    cells.push(cell);
+  }
+
+  return cells;
+}
+
+function trimEnd(s: string): string {
+  const trimmed = s.trim();
+
+  if (trimmed.length === 0) {
+    return '';
+  }
+
+  return s.slice(0, s.indexOf(trimmed) + trimmed.length);
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
 /**
-* getColumnWidths parses the provided line and returns the associated column widths.
-* 
-* @param line The separator line to parse for the column widths.
-* @returns The column widths for the provided line, or an empty array if the line is invalid. 
-*/
-export default function getColumnWidths(
-    line: string):
-    number[]
-{
-    // try to parse as a row separator line
-    let columnMatch = line
-        .substr(1)
-        .match(/[:-][-]+[:-]\+/g);
+ * getColumnWidths parses the provided line and returns the associated column widths.
+ *
+ * @param line The separator line to parse for the column widths.
+ * @returns The column widths for the provided line, or an empty array if the line is invalid.
+ */
+export default function getColumnWidths(line: string): number[] {
+  // try to parse as a row separator line
+  let columnMatch = line.substr(1).match(/[:-][-]+[:-]\+/g);
 
-    if (columnMatch == null)
-    {
-        // try to parse as a header separator line
-        columnMatch = line
-            .substr(1)
-            .match(/[:=][=]+[:=]\+/g);
-    }
+  if (columnMatch === null) {
+    // try to parse as a header separator line
+    columnMatch = line.substr(1).match(/[:=][=]+[:=]\+/g);
+  }
 
-    if (columnMatch == null)
-    {
-        return [];
-    }
+  if (columnMatch === null) {
+    return [];
+  }
 
-    return columnMatch.map(s => s.length);
-}
+  return columnMatch.map(s => s.length);
+}
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/EmitTable.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/EmitTable.ts`

 * *Files 15% similar despite different names*

```diff
@@ -1,110 +1,116 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
-import * as MarkdownIt from "markdown-it";
-import IState from "../../interfaces/markdown-it/IState";
-import getCells from "../gridtables/GetCells";
-import ColumnAlignments from "./ColumnAlignments";
-import ParseTableResult from "./ParseTableResult";
+import * as MarkdownIt from 'markdown-it';
+import IState from '../../interfaces/markdown-it/IState';
+import getCells from '../gridtables/GetCells';
+import ColumnAlignments from './ColumnAlignments';
+import ParseTableResult from './ParseTableResult';
 
 export default function emitTable(
-    md: MarkdownIt,
-    state: IState,
-    result: ParseTableResult)
-{
-    let offsets = result.SeparatorLineOffsets;
+  md: MarkdownIt,
+  state: IState,
+  result: ParseTableResult
+) {
+  let offsets = result.SeparatorLineOffsets;
+
+  let token = state.push('table_open', 'table', 1);
+  token.map = [offsets[0], offsets[offsets.length - 1]];
+
+  if (result.HeaderLines.length > 0) {
+    // emit table header
+    const token = state.push('thead_open', 'thead', 1);
+    token.map = [offsets[0], offsets[1]];
+
+    const cells = getCells(result.HeaderLines);
+
+    processRow(
+      md,
+      state,
+      'th',
+      result.ColumnAlignments,
+      offsets[0],
+      offsets[1],
+      cells
+    );
+
+    state.push('thead_close', 'thead', -1);
+
+    offsets = offsets.slice(1);
+  }
+
+  // emit table body
+  token = state.push('tbody_open', 'tbody', 1);
+  token.map = [offsets[0], offsets[offsets.length - 1]];
+
+  for (let i = 0; i < result.RowLines.length; i++) {
+    const cells = getCells(result.RowLines[i]);
+
+    processRow(
+      md,
+      state,
+      'td',
+      result.ColumnAlignments,
+      offsets[i],
+      offsets[i + 1],
+      cells
+    );
+  }
 
-    let token = state.push('table_open', 'table', 1);
-    token.map = [offsets[0], offsets[offsets.length - 1]];
+  state.push('tbody_close', 'tbody', -1);
 
-    if (result.HeaderLines.length > 0)
-    {
-        // emit table header
-        const token = state.push('thead_open', 'thead', 1);
-        token.map = [offsets[0], offsets[1]];
-
-        const cells = getCells(result.HeaderLines);
-
-        processRow(md, state, 'th', result.ColumnAlignments, offsets[0], offsets[1], cells);
+  state.push('table_close', 'table', -1);
+}
 
-        state.push('thead_close', 'thead', -1);
+function processRow(
+  md: MarkdownIt,
+  state: IState,
+  tag: string,
+  columnAlignments: ColumnAlignments[],
+  lineBegin: number,
+  lineEnd: number,
+  cells: string[][]
+) {
+  const token = state.push('tr_open', 'tr', 1);
+  token.map = [lineBegin, lineEnd];
+
+  for (let i = 0; i < cells.length; i++) {
+    const token = state.push(tag + '_open', tag, 1);
+    token.map = [lineBegin + 1, lineEnd - 1];
 
-        offsets = offsets.slice(1);
+    if (columnAlignments[i] !== ColumnAlignments.None) {
+      token.attrSet('style', `text-align: ${columnAlignments[i]};`);
     }
 
-    // emit table body
-    token = state.push('tbody_open', 'tbody', 1);
-    token.map = [offsets[0], offsets[offsets.length - 1]];
-
-    for (let i = 0; i < result.RowLines.length; i++)
-    {
-        let cells = getCells(result.RowLines[i]);
-
-        processRow(md, state, 'td', result.ColumnAlignments, offsets[i], offsets[i + 1], cells);
+    if (cells[i].length === 0) {
+      // empty cell
+    } else if (cells[i].length === 1) {
+      // single line cell -> emit as inline markdown
+      const token = state.push('inline', '', 0);
+      token.content = cells[i][0].trim();
+      token.children = [];
+    } else {
+      // multi line cell -> render and emit as html
+      let cell = md.render(cells[i].join('\r\n')).trim();
+
+      // remove single p tag because we're in a table cell
+      if (
+        cell.slice(0, 3) === '<p>' &&
+        cell.slice(-4) === '</p>' &&
+        cell.indexOf('<p>', 3) === -1
+      ) {
+        cell = cell.slice(3, cell.length - 4);
+      }
+
+      const token = state.push('html_block', '', 0);
+      token.content = cell;
+      token.children = [];
     }
 
-    state.push('tbody_close', 'tbody', -1);
+    state.push(tag + '_close', tag, -1);
+  }
 
-    state.push('table_close', 'table', -1);
+  state.push('tr_close', 'tr', -1);
 }
-
-function processRow(
-    md: MarkdownIt,
-    state: IState,
-    tag: string,
-    columnAlignments: ColumnAlignments[],
-    lineBegin: number,
-    lineEnd: number,
-    cells: string[][])
-{
-    let token = state.push('tr_open', 'tr', 1);
-    token.map = [lineBegin, lineEnd];
-
-    for (let i = 0; i < cells.length; i++)
-    {
-        let token = state.push(tag + '_open', tag, 1);
-        token.map = [lineBegin + 1, lineEnd - 1];
-
-        if (columnAlignments[i] !== ColumnAlignments.None)
-        {
-            token.attrSet("style", `text-align: ${columnAlignments[i]};`);
-        }
-
-        if (cells[i].length === 0)
-        {
-            // empty cell
-        }
-        else if (cells[i].length === 1)
-        {
-            // single line cell -> emit as inline markdown
-            let token = state.push('inline', '', 0);
-            token.content = cells[i][0].trim();
-            token.children = [];
-        }
-        else
-        {
-            // multi line cell -> render and emit as html
-            let cell = md
-                .render(cells[i].join('\r\n'))
-                .trim();
-
-            // remove single p tag because we're in a table cell
-            if ((cell.slice(0, 3) === '<p>') &&
-                (cell.slice(-4) === '</p>') &&
-                (cell.indexOf('<p>', 3) === -1))
-            {
-                cell = cell.slice(3, cell.length - 4);
-            }
-
-            let token = state.push('html_block', '', 0);
-            token.content = cell;
-            token.children = [];
-        }
-
-        state.push(tag + '_close', tag, -1);
-    }
-
-    state.push('tr_close', 'tr', -1);
-}
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
-import IState from "../../interfaces/markdown-it/IState";
+import IState from '../../interfaces/markdown-it/IState';
 
 /**
  * Returns the char code of the character at the start of the current line,
  * or -1 if this is not available (e.g. on an empty line).
- * 
+ *
  * @param state The Markdown It state.
  */
 export default function getCharCodeAtStartOfLine(
-    state: IState,
-    line: number
-): number
-{
-    const pos =
-        state.bMarks[line] +
-        state.tShift[line];
+  state: IState,
+  line: number
+): number {
+  const pos = state.bMarks[line] + state.tShift[line];
 
-    if (pos >= state.eMarks[line])
-    {
-        return -1;
-    }
+  if (pos >= state.eMarks[line]) {
+    return -1;
+  }
 
-    return state.src.charCodeAt(pos);
+  return state.src.charCodeAt(pos);
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/ParseTable.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/ParseTable.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,251 +1,217 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
-import wcwidth from "wcwidth";
-import IState from "../../interfaces/markdown-it/IState";
-import getColumnWidths from "../gridtables/GetColumnWidths";
-import ColumnAlignments from "./ColumnAlignments";
-import getLine from "./GetLine";
-import ParseTableResult from "./ParseTableResult";
+import wcwidth from 'wcwidth';
+import IState from '../../interfaces/markdown-it/IState';
+import getColumnWidths from '../gridtables/GetColumnWidths';
+import ColumnAlignments from './ColumnAlignments';
+import getLine from './GetLine';
+import ParseTableResult from './ParseTableResult';
 
 export default function parseTable(
-    state: IState,
-    startLine: number,
-    endLine: number):
-    ParseTableResult
-{
-    const result = new ParseTableResult();
-
-    let rowLine = getLine(state, startLine);
-
-    if (rowLine.charAt(0) !== '+')
-    {
-        // line does not start with a '+'
-        return result;
-    }
+  state: IState,
+  startLine: number,
+  endLine: number
+): ParseTableResult {
+  const result = new ParseTableResult();
 
-    result.ColumnWidths = getColumnWidths(rowLine);
+  let rowLine = getLine(state, startLine);
 
-    if (result.ColumnWidths.length === 0)
-    {
-        // no columns found
-        return result;
-    }
+  if (rowLine.charAt(0) !== '+') {
+    // line does not start with a '+'
+    return result;
+  }
 
-    // initialize column alignments
-    result.ColumnAlignments = result.ColumnWidths
-        .map(_ => ColumnAlignments.None);
-
-    if (rowLine.indexOf(':') >= 0)
-    {
-        // column alignment specifiers present in first row line
-        result.HeaderLess = true;
-
-        // set column alignments
-        result.ColumnAlignments = getColumnAlignments(
-            rowLine,
-            result.ColumnWidths);
+  result.ColumnWidths = getColumnWidths(rowLine);
 
-        // remove alignment specifiers for further matching
-        rowLine = rowLine.replace(/[:]/g, '-');
-    }
+  if (result.ColumnWidths.length === 0) {
+    // no columns found
+    return result;
+  }
 
-    // create header line matcher
-    const headerLineMatcher = new RegExp(
-        '^\\+' +
-        result.ColumnWidths
-            .map(w => `[=:][=]{${w - 3}}[=:]\\+`)
-            .join('') +
-        '$');
-
-    // build column offsets
-    result.ColumnOffsets = [0];
-
-    for (let i = 0; i < result.ColumnWidths.length - 1; i++)
-    {
-        result.ColumnOffsets.push(
-            result.ColumnOffsets[i] +
-            result.ColumnWidths[i]);
-    }
+  // initialize column alignments
+  result.ColumnAlignments = result.ColumnWidths.map(
+    () => ColumnAlignments.None
+  );
+
+  if (rowLine.indexOf(':') >= 0) {
+    // column alignment specifiers present in first row line
+    result.HeaderLess = true;
+
+    // set column alignments
+    result.ColumnAlignments = getColumnAlignments(rowLine, result.ColumnWidths);
+
+    // remove alignment specifiers for further matching
+    rowLine = rowLine.replace(/[:]/g, '-');
+  }
+
+  // create header line matcher
+  const headerLineMatcher = new RegExp(
+    '^\\+' +
+      result.ColumnWidths.map(w => `[=:][=]{${w - 3}}[=:]\\+`).join('') +
+      '$'
+  );
+
+  // build column offsets
+  result.ColumnOffsets = [0];
+
+  for (let i = 0; i < result.ColumnWidths.length - 1; i++) {
+    result.ColumnOffsets.push(result.ColumnOffsets[i] + result.ColumnWidths[i]);
+  }
+
+  // create cell line matcher
+  const cellLineMatcher = new RegExp(
+    '^\\|' +
+      result.ColumnWidths.map(
+        w => `([^|]{${Math.ceil((w - 1) / 2)},${w - 1}})\\|`
+      ).join('') +
+      '$'
+  );
+
+  // save first separator line offset
+  result.SeparatorLineOffsets.push(startLine);
+
+  // continue to scan until a complete table is found, or an invalid line is encountered
+  let currentRow: string[][] = [];
+  let currentLine = startLine + 1;
+
+  for (; currentLine <= endLine; currentLine++) {
+    const line = getLine(state, currentLine);
+
+    if (line.charCodeAt(0) === 0x2b) {
+      // '+'
+      // separator line
+      if (currentRow.length === 0) {
+        // no row lines since last separator -> invalid table
+        return result;
+      }
 
-    // create cell line matcher
-    const cellLineMatcher = new RegExp(
-        '^\\|' +
-        result.ColumnWidths
-            .map(w => `([^|]{${Math.ceil((w - 1) / 2)},${w - 1}})\\|`)
-            .join('') +
-        '$');
-
-    // save first separator line offset
-    result.SeparatorLineOffsets.push(startLine);
-
-    // continue to scan until a complete table is found, or an invalid line is encountered
-    let currentRow: string[][] = [];
-    let currentLine = startLine + 1;
-
-    for (; currentLine <= endLine; currentLine++)
-    {
-        const line = getLine(state, currentLine);
-
-        if (line.charCodeAt(0) === 0x2B) // '+'
-        {
-            // separator line
-            if (currentRow.length === 0)
-            {
-                // no row lines since last separator -> invalid table
-                return result;
-            }
-
-            // save separator line offset
-            result.SeparatorLineOffsets.push(currentLine);
-
-            if (line === rowLine)
-            {
-                // new regular row
-                result.RowLines.push(currentRow);
-
-                if (result.HeaderLines.length === 0)
-                {
-                    result.HeaderLess = true;
-                }
-            } else if (!result.HeaderLess &&
-                line.match(headerLineMatcher))
-            {
-                // found header line
-                if (result.HeaderLines.length > 0 ||
-                    result.RowLines.length > 0)
-                {
-                    // header already found, or not the first row -> invalid table
-                    return result;
-                }
-
-                // header row
-                result.HeaderLines = currentRow;
-
-                if (line.indexOf(':') >= 0)
-                {
-                    // set column alignments
-                    result.ColumnAlignments = getColumnAlignments(
-                        line,
-                        result.ColumnWidths);
-                }
-            } else
-            {
-                // not a header or regular row -> invalid table
-                return result;
-            }
+      // save separator line offset
+      result.SeparatorLineOffsets.push(currentLine);
 
-            // reset current row
-            currentRow = [];
-        }
-        else if (line.charCodeAt(0) === 0x7C) // '|'
-        {
-            // cell line
-
-            const matches = line.match(cellLineMatcher);
-
-            if (matches === null)
-            {
-                // cell line does not match -> invalid table
-                return result;
-            }
-
-            const cells = validateColumnWidths(
-                matches,
-                result.ColumnWidths);
-
-            if (cells === null)
-            {
-                // cell line does not match -> invalid table
-                return result;
-            }
+      if (line === rowLine) {
+        // new regular row
+        result.RowLines.push(currentRow);
 
-            // add the line to the current row
-            currentRow.push(cells);
+        if (result.HeaderLines.length === 0) {
+          result.HeaderLess = true;
+        }
+      } else if (!result.HeaderLess && line.match(headerLineMatcher)) {
+        // found header line
+        if (result.HeaderLines.length > 0 || result.RowLines.length > 0) {
+          // header already found, or not the first row -> invalid table
+          return result;
         }
-        else
-        {
-            // not a separator or cell line, check if we have a complete table
-            if (currentRow.length === 0 &&
-                ((result.HeaderLines.length > 0) ||
-                    (result.RowLines.length > 0)))
-            {
-                // found a complete table
-                break;
-            }
 
-            return result;
+        // header row
+        result.HeaderLines = currentRow;
+
+        if (line.indexOf(':') >= 0) {
+          // set column alignments
+          result.ColumnAlignments = getColumnAlignments(
+            line,
+            result.ColumnWidths
+          );
         }
+      } else {
+        // not a header or regular row -> invalid table
+        return result;
+      }
+
+      // reset current row
+      currentRow = [];
+    } else if (line.charCodeAt(0) === 0x7c) {
+      // '|'
+      // cell line
+
+      const matches = line.match(cellLineMatcher);
+
+      if (matches === null) {
+        // cell line does not match -> invalid table
+        return result;
+      }
+
+      const cells = validateColumnWidths(matches, result.ColumnWidths);
+
+      if (cells === null) {
+        // cell line does not match -> invalid table
+        return result;
+      }
+
+      // add the line to the current row
+      currentRow.push(cells);
+    } else {
+      // not a separator or cell line, check if we have a complete table
+      if (
+        currentRow.length === 0 &&
+        (result.HeaderLines.length > 0 || result.RowLines.length > 0)
+      ) {
+        // found a complete table
+        break;
+      }
+
+      return result;
     }
+  }
 
-    result.CurrentLine = currentLine;
+  result.CurrentLine = currentLine;
 
-    result.Success = true;
+  result.Success = true;
 
-    return result;
+  return result;
 }
 
 function getColumnAlignments(
-    line: string,
-    columnWidths: number[]):
-    ColumnAlignments[]
-{
-
-    let alignments: ColumnAlignments[] = [];
-
-    let left = 1;
-    let right = -1;
-
-    for (let i = 0; i < columnWidths.length; i++)
-    {
-        right += columnWidths[i];
-
-        let alignment = ColumnAlignments.None;
-
-        if (line.charAt(right) === ':')
-        {
-            if (line.charAt(left) === ':')
-            {
-                alignment = ColumnAlignments.Center;
-            } else
-            {
-                alignment = ColumnAlignments.Right;
-            }
-        } else if (line.charAt(left) === ':')
-        {
-            alignment = ColumnAlignments.Left;
-        }
+  line: string,
+  columnWidths: number[]
+): ColumnAlignments[] {
+  const alignments: ColumnAlignments[] = [];
+
+  let left = 1;
+  let right = -1;
 
-        alignments.push(alignment);
+  for (let i = 0; i < columnWidths.length; i++) {
+    right += columnWidths[i];
 
-        left += columnWidths[i];
+    let alignment = ColumnAlignments.None;
+
+    if (line.charAt(right) === ':') {
+      if (line.charAt(left) === ':') {
+        alignment = ColumnAlignments.Center;
+      } else {
+        alignment = ColumnAlignments.Right;
+      }
+    } else if (line.charAt(left) === ':') {
+      alignment = ColumnAlignments.Left;
     }
 
-    return alignments;
+    alignments.push(alignment);
+
+    left += columnWidths[i];
+  }
+
+  return alignments;
 }
 
 function validateColumnWidths(
-    matches: RegExpMatchArray,
-    columnWidths: number[],
-): string[] | null
-{
-    const cells: string[] = [];
-
-    for (var i = 0; i < columnWidths.length; i++)
-    {
-        const cell = matches[i + 1];
-
-        const columnWidth = wcwidth(cell) + 1; // add 1 for separator
-
-        if (columnWidth !== columnWidths[i])
-        {
-            return null;
-        }
+  matches: RegExpMatchArray,
+  columnWidths: number[]
+): string[] | null {
+  const cells: string[] = [];
 
-        cells.push(cell);
+  for (let i = 0; i < columnWidths.length; i++) {
+    const cell = matches[i + 1];
+
+    const columnWidth = wcwidth(cell) + 1; // add 1 for separator
+
+    if (columnWidth !== columnWidths[i]) {
+      return null;
     }
 
-    return cells;
-}
+    cells.push(cell);
+  }
+
+  return cells;
+}
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
-import ColumnAlignments from "./ColumnAlignments";
+import ColumnAlignments from './ColumnAlignments';
 
-export default class ParseTableResult
-{
-    Success: boolean = false;
+export default class ParseTableResult {
+  Success = false;
 
-    ColumnWidths: number[] = [];
+  ColumnWidths: number[] = [];
 
-    ColumnOffsets: number[] = [];
+  ColumnOffsets: number[] = [];
 
-    ColumnAlignments: ColumnAlignments[] = [];
+  ColumnAlignments: ColumnAlignments[] = [];
 
-    HeaderLess: boolean = false;
+  HeaderLess = false;
 
-    HeaderLines: string[][] = [];
+  HeaderLines: string[][] = [];
 
-    RowLines: string[][][] = [];
+  RowLines: string[][][] = [];
 
-    SeparatorLineOffsets: number[] = [];
+  SeparatorLineOffsets: number[] = [];
 
-    CurrentLine: number = 0;
+  CurrentLine = 0;
 }
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts` & `jupyterlab_quarto-0.2.2/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 /*---------------------------------------------------------------------------------------------
  *  Copyright (c) Bas Verweij. All rights reserved.
  *  Licensed under the MIT License. See LICENSE in the project root for license information.
  *--------------------------------------------------------------------------------------------*/
 
-import IState from "./IState";
+import IState from './IState';
 
 type TRuleFunction = (
-    state: IState,
-    startLine: number,
-    endLine: number,
-    silent: boolean) => boolean;
+  state: IState,
+  startLine: number,
+  endLine: number,
+  silent: boolean
+) => boolean;
 
-export default TRuleFunction;
+export default TRuleFunction;
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/mermaid/index.ts` & `jupyterlab_quarto-0.2.2/src/plugins/mermaid/index.ts`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,82 @@
 /* eslint-disable @typescript-eslint/no-explicit-any */
-import MarkdownIt from "markdown-it";
-import Mermaid from "mermaid";
+import MarkdownIt from 'markdown-it';
+import Mermaid from 'mermaid';
 
-export default function mermaidPlugin(md: MarkdownIt, options: { dark?: boolean}) {
-
-
-  const kLang = "mermaid";
-  const kContainer = "quarto-mermaid";
+export default function mermaidPlugin(
+  md: MarkdownIt,
+  options: { dark?: boolean }
+) {
+  const kLang = 'mermaid';
+  const kContainer = 'quarto-mermaid';
 
   Mermaid.initialize({
-    securityLevel: "loose",
-    theme: options.dark ? "dark" : "default",
-    ...options,
+    securityLevel: 'loose',
+    theme: options.dark ? 'dark' : 'default',
+    ...options
   });
 
   const defaultFenceRenderer = md.renderer.rules.fence;
 
   // Render custom code types as SVGs, letting the fence parser do all the heavy lifting.
   function mermaidFenceRenderer(
     tokens: any[],
     idx: number,
     options: any,
     env: any,
     slf: any
   ) {
     const token = tokens[idx];
-    if (token.info === kLang || (token.attrs !== null && token.attrs.length === 1 && token.attrs[0][0] === kLang))  {
-      let imageHTML = "";
+    if (
+      token.info === kLang ||
+      (token.attrs !== null &&
+        token.attrs.length === 1 &&
+        token.attrs[0][0] === kLang)
+    ) {
+      let imageHTML = '';
       const imageAttrs: string[][] = [];
-  
+
       // Create element to render into
-      const element = document.createElement("div");
+      const element = document.createElement('div');
       document.body.appendChild(element);
-  
+
       // Render with Mermaid
       try {
         Mermaid.mermaidAPI.render(
           kContainer,
           token.content,
           (html: string) => {
             // We need to forcibly extract the max-width/height attributes to set on img tag
             const mermaidEl = document.getElementById(kContainer);
             if (mermaidEl !== null) {
               imageAttrs.push([
-                "style",
-                `max-width:${mermaidEl.style.maxWidth};max-height:${mermaidEl.style.maxHeight}`,
+                'style',
+                `max-width:${mermaidEl.style.maxWidth};max-height:${mermaidEl.style.maxHeight}`
               ]);
             }
             // Store HTML
             imageHTML = html;
           },
           element
         );
       } catch (e) {
-        return `<pre>Failed to render mermaid diagram.${e}</pre>`
+        return `<pre>Failed to render mermaid diagram.${e}</pre>`;
       } finally {
         element.remove();
       }
-  
+
       // Store encoded image data
-      imageAttrs.push(["src", `data:image/svg+xml,${encodeURIComponent(imageHTML)}`]);
+      imageAttrs.push([
+        'src',
+        `data:image/svg+xml,${encodeURIComponent(imageHTML)}`
+      ]);
       return `<img ${slf.renderAttrs({ attrs: imageAttrs })}>`;
     } else {
       if (defaultFenceRenderer !== undefined) {
         return defaultFenceRenderer(tokens, idx, options, env, slf);
       }
       // Missing fence renderer!
-      return "";
+      return '';
     }
   }
   md.renderer.rules.fence = mermaidFenceRenderer;
-}
+}
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/utils/html.ts` & `jupyterlab_quarto-0.2.2/src/plugins/utils/html.ts`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 /*
-* html.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * html.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 
-import Token from "markdown-it/lib/token";
-import { readAttrValue } from "./markdownit";
+import Token from 'markdown-it/lib/token';
+import { readAttrValue } from './markdownit';
 
 export interface DecoratorOptions {
   customClass?: string;
   hide: {
     id?: boolean;
     classes?: boolean;
     attributes?: boolean;
-  }
+  };
 }
 
 export const decorator = (contents: string[], customClass?: string) => {
   if (contents.length > 0) {
     // Provide a decorator with the attributes
-    return `<div class="quarto-attribute-decorator${customClass ? ' ' + customClass : ""}">${contents.map(decoratorSpan).join("")}</div>`  
+    return `<div class="quarto-attribute-decorator${
+      customClass ? ' ' + customClass : ''
+    }">${contents.map(decoratorSpan).join('')}</div>`;
   } else {
     // There is no decorator - no attributes
-    return "";
+    return '';
   }
-}
+};
 
-export const attributeDecorator = (token: Token, options?: DecoratorOptions) => {
+export const attributeDecorator = (
+  token: Token,
+  options?: DecoratorOptions
+) => {
   // id
-  const id = readAttrValue("id", token.attrs);
-  
+  const id = readAttrValue('id', token.attrs);
+
   // classes
-  const clz = readAttrValue("class", token.attrs);
+  const clz = readAttrValue('class', token.attrs);
 
   // other attributes
-  const otherAttrs = token.attrs?.filter((attr) => { return attr[0] !== "id" && attr[0] !== "class"});
+  const otherAttrs = token.attrs?.filter(attr => {
+    return attr[0] !== 'id' && attr[0] !== 'class';
+  });
 
   // Create a decorator for the div
   const contents: string[] = [];
   if (id && !options?.hide.id) {
     contents.push(`#${id}`);
-  } 
+  }
   if (clz && !options?.hide.classes) {
-    const clzStr = clz.split(" ").map((cls) => `.${cls}`).join(" ");
+    const clzStr = clz
+      .split(' ')
+      .map(cls => `.${cls}`)
+      .join(' ');
     contents.push(clzStr);
   }
   if (otherAttrs && otherAttrs.length > 0 && !options?.hide.attributes) {
-    const otherAttrStr = otherAttrs?.map((attr) => {
-      return `${attr[0]}="${attr[1]}"`
-    }).join(" ");
+    const otherAttrStr = otherAttrs
+      ?.map(attr => {
+        return `${attr[0]}="${attr[1]}"`;
+      })
+      .join(' ');
     contents.push(otherAttrStr);
   }
   return decorator(contents, options?.customClass);
-}
+};
 
 const decoratorSpan = (contents: string) => {
-  return `<span class="quarto-attribute-decorator-content">${contents}</span>`
-}
-
+  return `<span class="quarto-attribute-decorator-content">${contents}</span>`;
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/plugins/utils/markdownit.ts` & `jupyterlab_quarto-0.2.2/src/plugins/utils/markdownit.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 /*
-* markdownit.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * markdownit.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 
 export const hasClass = (clz: string, attrs: null | [string, string][]) => {
   if (attrs === null) {
-    return false
+    return false;
   }
 
-  const classes = readAttrValue("class", attrs);
+  const classes = readAttrValue('class', attrs);
   if (classes === null) {
     return false;
   } else {
-    return classes?.split(" ").includes(clz);
+    return classes?.split(' ').includes(clz);
   }
+};
 
-
-}
-
-export const readAttrValue = (name: string, attrs: null | [string, string][]) => {
+export const readAttrValue = (
+  name: string,
+  attrs: null | [string, string][]
+) => {
   if (attrs === null) {
     return undefined;
   }
 
-  const attr = attrs.find((attr) => { return attr[0] === name; });
+  const attr = attrs.find(attr => {
+    return attr[0] === name;
+  });
   return attr ? attr[1] : undefined;
-}
+};
 
-export const addClass = (clz: string, attrs: null | [string, string][]): [string, string][] => {
+export const addClass = (
+  clz: string,
+  attrs: null | [string, string][]
+): [string, string][] => {
   if (attrs === null) {
-    attrs = []
-    attrs.push(["class", clz])
+    attrs = [];
+    attrs.push(['class', clz]);
     return attrs;
   } else {
-    const clzIdx = attrs.findIndex((attr) => attr[0] === "class");
+    const clzIdx = attrs.findIndex(attr => attr[0] === 'class');
     if (clzIdx >= 0) {
       const currentClz = attrs[clzIdx];
-      attrs[clzIdx] = ["class", `${currentClz[1]} ${clz}`.trim()];
+      attrs[clzIdx] = ['class', `${currentClz[1]} ${clz}`.trim()];
       return attrs;
     } else {
-      attrs.push(["class", clz])
-      return attrs; 
+      attrs.push(['class', clz]);
+      return attrs;
     }
   }
-}
+};
```

### Comparing `jupyterlab_quarto-0.1.45/src/providers/divs.ts` & `jupyterlab_quarto-0.2.2/src/providers/divs.ts`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /*
-* callouts.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
-import { divPlugin } from "../plugins/divs";
-import { markdownItExtension } from "./provider";
+ * callouts.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
+import { divPlugin } from '../plugins/divs';
+import { markdownItExtension } from './provider';
 
 export const divs = markdownItExtension({
   id: '@quarto/divs',
   title: 'Pandoc fenced divs',
   plugin: async () => {
     return [divPlugin];
   },
   hooks: {
     preParse: {
       run: (content: string) => {
         // Detect close divs that are directly after text (e.g. not back to back whitespace)
-        // and add a whitespace. This will cause the close div to become a 'block' 
+        // and add a whitespace. This will cause the close div to become a 'block'
         // rather than appearing as the end of the paragraph block
-        const blockedDivs = content.replace(kCloseDivNoBlock, `$1\n\n$2`);
-        return Promise.resolve(blockedDivs)
+        const blockedDivs = content.replace(kCloseDivNoBlock, '$1\n\n$2');
+        return Promise.resolve(blockedDivs);
       }
     }
   }
 });
 
-const kCloseDivNoBlock = /([^\s])\n(:::+(?:\{.*\})?)/gm;
+const kCloseDivNoBlock = /([^\s])\n(:::+(?:\{.*\})?)/gm;
```

### Comparing `jupyterlab_quarto-0.1.45/src/providers/math.ts` & `jupyterlab_quarto-0.2.2/src/providers/math.ts`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 /*
-* math.ts
-*
-* Copyright (C) 2020-2023 Posit Software, PBC
-*
-*/
+ * math.ts
+ *
+ * Copyright (C) 2020-2023 Posit Software, PBC
+ *
+ */
 import { mathjaxPlugin } from '../plugins/math';
 import { markdownItExtension } from './provider';
 
 export const math = markdownItExtension({
   id: '@quarto/math',
   title: 'LaTex Math',
   plugin: async () => {
     return [mathjaxPlugin];
   },
   hooks: {
     postRender: {
       run: (node: HTMLElement) => {
-
         // Inject mathjax
-        const mathjaxId = "MathJax-script";
+        const mathjaxId = 'MathJax-script';
         const mathJaxScript = document.getElementById(mathjaxId);
         if (!mathJaxScript) {
-
-          const configEl = document.createElement("script");
+          const configEl = document.createElement('script');
           configEl.innerText = `
 
 MathJax = {
   svg: {
     fontCache: 'global'
   },
   startup: {
@@ -83,30 +81,35 @@
           }    
         });
       });
     },
   }
 };`;
           document.head.appendChild(configEl);
-          
 
-          const polyFillEl = document.createElement("script");
-          polyFillEl.setAttribute("src", "https://polyfill.io/v3/polyfill.min.js?features=es6");
+          const polyFillEl = document.createElement('script');
+          polyFillEl.setAttribute(
+            'src',
+            'https://polyfill.io/v3/polyfill.min.js?features=es6'
+          );
           document.head.appendChild(polyFillEl);
 
-          const scriptEl = document.createElement("script");
+          const scriptEl = document.createElement('script');
           scriptEl.id = mathjaxId;
-          scriptEl.setAttribute("src", "https://cdn.jsdelivr.net/npm/mathjax@3.0.1/es5/tex-mml-chtml.js");
+          scriptEl.setAttribute(
+            'src',
+            'https://cdn.jsdelivr.net/npm/mathjax@3.0.1/es5/tex-mml-chtml.js'
+          );
           document.head.appendChild(scriptEl);
         }
 
         return Promise.resolve();
       }
     }
   }
 });
 
 /*
 <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
 <script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
 
-*/
+*/
```

### Comparing `jupyterlab_quarto-0.1.45/style/base.css` & `jupyterlab_quarto-0.2.2/style/base.css`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 }
 
 .quarto-meta {
   margin-bottom: 1.4em;
 }
 
 .quarto-meta-padded {
-  padding-top: .4em;
+  padding-top: 0.4em;
 }
 
 .quarto-meta p.quarto-meta-title {
   text-transform: uppercase;
   font-size: 0.8em;
 }
 
@@ -29,23 +29,23 @@
   margin-bottom: 0;
 }
 
 .quarto-orcid {
   text-decoration: none;
 }
 
-.quarto-orcid i:before {
+.quarto-orcid i::before {
   margin-left: 0.25em;
   height: 1rem;
   width: 1rem;
   display: inline-block;
-  content: "";
+  content: '';
   background-repeat: no-repeat;
   background-size: 1rem 1rem;
-  background-image: url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAALVBMVEUAAACmzjmmzjmmzjmmzjmmzjn////0+ebj8MHe7bXT55y82mus0UWmzjmSwCmNJ4LqAAAABnRSTlMAIGC/z+8mlFLTAAAAaElEQVR42k2OsQmAMBRET3CAFG5gbWMv6CBpRT44knM4hU3ESl6bLs5gEUW7x3GPO0k1tJJUAQxS4S3B4VRiCejVcCU2gjosjtO2CyymdSHDOT/A/Eu63NnVZCuoBIBehQc43Df63rgBoFJNFnlCBV4AAAAASUVORK5CYII=");
+  background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQBAMAAADt3eJSAAAALVBMVEUAAACmzjmmzjmmzjmmzjmmzjn////0+ebj8MHe7bXT55y82mus0UWmzjmSwCmNJ4LqAAAABnRSTlMAIGC/z+8mlFLTAAAAaElEQVR42k2OsQmAMBRET3CAFG5gbWMv6CBpRT44knM4hU3ESl6bLs5gEUW7x3GPO0k1tJJUAQxS4S3B4VRiCejVcCU2gjosjtO2CyymdSHDOT/A/Eu63NnVZCuoBIBehQc43Df63rgBoFJNFnlCBV4AAAAASUVORK5CYII=');
 }
 
 .quarto-frontmatter {
   font-size: 0.9em !important;
   line-height: 0.9em !important;
 }
 
@@ -54,15 +54,15 @@
 }
 
 /* Decorated Divs */
 
 .quarto-div {
   border: solid 1px var(--jp-border-color0);
   border-radius: 3px;
-  background-color: #EEEEEE33;
+  background-color: #eee3;
   padding: 1em;
   margin-bottom: 1em;
 }
 
 .quarto-attribute-decorator + h1,
 .quarto-attribute-decorator + h2,
 .quarto-attribute-decorator + h3,
@@ -96,176 +96,177 @@
   padding-bottom: 2px;
   padding-left: 7px;
   padding-right: 7px;
   white-space: nowrap;
 }
 
 /* Cites and Xrefs */
-.jp-RenderedHTMLCommon :not(pre) > code.cite { 
+.jp-RenderedHTMLCommon :not(pre) > code.cite {
   color: var(--jp-content-link-color);
   padding-left: 1px;
   padding-right: 1px;
 }
 
 /* Code Blocks */
 .jp-RenderedHTMLCommon pre,
 .jp-RenderedHTMLCommon > pre {
-  margin-left: .1em;
+  margin-left: 0.1em;
   margin-right: 0;
   padding: 0.5em;
   border: solid 1px var(--jp-border-color0);
   border-radius: 3px;
 }
 
 /* Tables */
 .quarto-rendered-md.jp-RenderedHTMLCommon table {
   margin-left: inherit;
   margin-right: inherit;
 }
 
 /* Callouts */
+
 /* TODO: Need to automate ingesting this */
 
 .callout {
   margin-top: 1em;
-  margin-bottom: 1em;  
-  border-radius: .25rem;
+  margin-bottom: 1em;
+  border-radius: 0.25rem;
 }
 
 .callout-header {
   display: flex;
   align-content: center;
   padding: 0.35em 0.75em;
-  opacity: 80%;
+  opacity: 0.8;
 }
 
 .callout-title-container {
   font-size: 1em;
   font-weight: 600;
 }
 
-body[data-jp-theme-light="false"] .callout-title-container {
+body[data-jp-theme-light='false'] .callout-title-container {
   color: var(--jp-input-background);
 }
 
-.callout.callout-style-default  div.callout-title {
+.callout.callout-style-default div.callout-title {
   border-bottom: none;
   font-weight: 600;
-  opacity: 85%;
+  opacity: 0.85;
   font-size: 0.9rem;
   padding-left: 0.5em;
   padding-right: 0.5em;
 }
 
 .callout.callout-style-default {
-  border-left: solid #acacac .3rem;
+  border-left: solid #acacac 0.3rem;
   border-right: solid 1px silver;
   border-top: solid 1px silver;
   border-bottom: solid 1px silver;
 }
 
 .callout .callout-body-container {
   padding: 0.75em;
   flex-grow: 1;
 }
+
 .callout .callout-body-container p:last-of-type {
   margin-bottom: 0;
 }
 
 .callout.callout-style-default .callout-body {
   font-size: 0.9rem;
   font-weight: 400;
 }
 
 .callout.callout-style-default div.callout-content {
   padding-left: 0.5em;
   padding-right: 0.5em;
 }
 
-.callout.callout-style-default .callout-icon::before {
-  height: 1rem;
-  width: 1rem;
-  display: inline-block;
-  content: "";
-  background-repeat: no-repeat;
-  background-size: 1rem 1rem;
-  margin-bottom: -3px;
-  padding-right: .4rem;
-}
-
 .callout-title {
-  display: flex
+  display: flex;
 }
-  
 
 /* Callout Types */
 
 div.callout-note {
   border-left-color: #4582ec !important;
 }
 
 div.callout-note .callout-icon::before {
   background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAAEU0lEQVRYCcVXTWhcVRQ+586kSUMMxkyaElstCto2SIhitS5Ek8xUKV2poatCcVHtUlFQk8mbaaziwpWgglJwVaquitBOfhQXFlqlzSJpFSpIYyXNjBNiTCck7x2/8/LeNDOZxDuEkgOXe++553zfefee+/OYLOXFk3+1LLrRdiO81yNqZ6K9cG0P3MeFaMIQjXssE8Z1JzLO9ls20MBZX7oG8w9GxB0goaPrW5aNMp1yOZIa7Wv6o2ykpLtmAPs/vrG14Z+6d4jpbSKuhdcSyq9wGMPXjonwmESXrriLzFGOdDBLB8Y6MNYBu0dRokSygMA/mrun8MGFN3behm6VVAwg4WR3i6FvYK1T7MHo9BK7ydH+1uurECoouk5MPRyVSBrBHMYwVobG2aOXM07sWrn5qgB60rc6mcwIDJtQrnrEr44kmy+UO9r0u9O5/YbkS9juQckLed3DyW2XV/qWBBB3ptvI8EUY3I9p/67OW+g967TNr3Sotn3IuVlfMLVnsBwH4fsnebJvyGm5GeIUA3jljERmrv49SizPYuq+z7c2H/jlGC+Ghhupn/hcapqmcudB9jwJ/3jvnvu6vu5lVzF1fXyZuZZ7U8nRmVzytvT+H3kilYvH09mLWrQdwFSsFEsxFVs5fK7A0g8gMZjbif4ACpKbjv7gNGaD8bUrlk8x+KRflttr22JEMRUbTUwwDQScyzPgedQHZT0xnx7ujw2jfVfExwYHwOsDTjLdJ2ebmeQIlJ7neo41s/DrsL3kl+W2lWvAga0tR3zueGr6GL78M3ifH0rGXrBC2aAR8uYcIA5gwV8zIE8onoh8u0Fca/ciF7j1uOzEnqcIm59sEXoGc0+z6+H45V1CvAvHcD7THztu669cnp+L0okAeIc6zjbM/24LgGM1gZk7jnRu1aQWoU9sfUOuhrmtaPIO3YY1KLLWZaEO5TKUbMY5zx8W9UJ6elpLwKXbsaZ4EFl7B4bMtDv0iRipKoDQT2sNQI9b1utXFdYisi+wzZ/ri/1m7QfDgEuvgUUEIJPq3DhX/5DWNqIXDOweC2wvIR90Oq3lDpdMIgD2r0dXvGdsEW5H6x6HLRJYU7C69VefO1x8Gde1ZFSJLfWS1jbCnhtOPxmpfv2LXOA2Xk2tvnwKKPFuZ/oRmwBwqRQDcKNeVQkYcOjtWVBuM/JuYw5b6isojIkYxyYAFn5K7ZBF10fea52y8QltAg6jnMqNHFBmGkQ1j+U43HMi2xMar1Nv0zGsf1s8nUsmUtPOOrbFIR8bHFDMB5zL13Gmr/kGlCkUzedTzzmzsaJXhYawnA3UmARpiYj5ooJZiUoxFRtK3X6pgNPv+IZVPcnwbOl6f+aBaO1CNvPW9n9LmCp01nuSaTRF2YxHqZ8DYQT6WsXT+RD6eUztwYLZ8rM+rcPxamv1VQzFUkzFXvkiVrySGQgJNvXHJAxiU3/NwiC03rSf05VBaPtu/Z7/B8Yn/w7eguloAAAAAElFTkSuQmCC');
 }
 
 div.callout-note .callout-header {
-  background-color: #dae6fb
+  background-color: #dae6fb;
 }
 
 div.callout-important {
   border-left-color: #d9534f !important;
 }
 
 div.callout-important .callout-icon::before {
   background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAAEKklEQVRYCcVXTWhcVRS+575MJym48A+hSRFr00ySRQhURRfd2HYjk2SSTokuBCkU2o0LoSKKraKIBTcuFCoidGFD08nkBzdREbpQ1EDNIv8qSGMFUboImMSZd4/f9zJv8ibJMC8xJQfO3HPPPef7zrvvvnvviIkpC9nsw0UttFunbUhpFzFtarSd6WJkStVMw5xyVqYTvkwfzuf/5FgtkVoB0729j1rjXwThS7Vio+Mo6DNnvLfahoZ+i/o32lULuJ3NNiz7q6+pyAUkJaFF6JwaM2lUJlV0MlnQn5aTRbEu0SEqHUa0A4AdiGuB1kFXRfVyg5d87+Dg4DL6m2TLAub60ilj7A1Ec4odSAc8X95sHh7+ZRPCFo6Fnp7HfU/fBng/hi10CjCnWnJjsxvDNxWw0NfV6Rv5GgP3I3jGWXumdTD/3cbEOP2ZbOZp69yniG3FQ9z1jD7bnBu9Fc2tKGC2q+uAJOQHBDRiZX1x36o7fWBs7J9ownbtO+n0/qWkvW7UPIfc37WgT6ZGR++EOJyeQDSb9UB+DZ1G6DdLDzyS+b/kBCYGsYgJbSQHuThGKRcw5xdeQf8YdNHsc6ePXrlSYMBuSIAFTGAtQo+VuALo4BX83N190NWZWbynBjhOHsmNfFWLeL6v+ynsA58zDvvAC8j5PkbOcXCMg2PZFk3q8MjI7WAG/Dp9AwP7jdGBOOQkAvlFUB+irtm16I1Zw9YBcpGTGXYmk3kQIC/Cds55l+iMI3jqhjAuaoe+am2Jw5GT3Nbz3CkE12NavmzN5+erJW7046n/CH1RO/RVa8lBLozXk9uqykkGAyRXLWlLv5jyp4RFsG5vGVzpDLnIjTWgnRy2Rr+tDKvRc7Y8AyZq10jj8DqXdnIRNtFZb+t/ZRtXcDiVnzpqx8mPcDWxgARUqx0W1QB9MeUZiNrV4qP+Ehc+BpNgATsTX8ozYKL2NtFYAHc84fG7ndxUPr+AR/iQSns7uSUufAymwDOb2+NjK27lEFocm/EE2WpyIy/Hi66MWuMKJn8RvxIcj87IM5Vh9663ziW36kR0HNenXuxmfaD8JC7tfKbrhFr7LiZCrMjrzTeGx+PmkosrkNzW94ObzwocJ7A1HokLolY+AvkTiD/q1H0cN48c5EL8Crkttsa/AXQVDmutfyku0E7jShx49XqV3MFK8IryDhYVbj7Sj2P2eBxwcXoe8T8idsKKPRcnZw1b+slFTubwUwhktrfnAt7J++jwQtLZcm3sr9LQrjRzz6cfMv9aLvgmnAGvpoaGLxM4mAEaLV7iAzQ3oU0IvD5x9ix3yF2RAAuYAOO2f7PEFWCXZ4C9Pb2UsgDeVnFSpbFK7/IWu7TPTvBqzbGdCHOJQSxiEjt6IyZmxQyEJHv6xyQsYk//moVFsN2zP6fRImjfq7/n/wFDguUQFNEwugAAAABJRU5ErkJggg==');
 }
 
 div.callout-important .callout-header {
-  background-color: #f7dddc
+  background-color: #f7dddc;
 }
 
 div.callout-warning {
   border-left-color: #f0ad4e !important;
 }
 
 div.callout-warning .callout-icon::before {
   background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAAETklEQVRYCeVWW2gcVRg+58yaTUnizqbipZeX4uWhBEniBaoUX1Ioze52t7sRq6APio9V9MEaoWlVsFasRq0gltaAPuxms8lu0gcviE/FFOstVbSIxgcv6SU7EZqmdc7v9+9mJtNks51NTUH84ed889/PP+cmxP+d5FIbMJmNbpREu4WUkiTtCicKny0l1pIKmBzovF2S+hIJHX8iEu3hZJ5lNZGqyRrGSIQpq15AzF28jgpeY6yk6GVdrfFqdrD6Iw+QlB8g0YS2g7dyQmXM/IDhBhT0UCiRf59lfqmmDvzRt6kByV/m4JjtzuaujMUM2c5Z2d6JdKrRb3K2q6mA+oYVz8JnDdKPmmNthzkAk/lN63sYPgevrguc72aZX/L9C6x09GYyxBgCX4NlvyGUHOKELlm5rXeR1kchuChJt4SSwyddZRXgvwMGvYo4QSlk3/zkHD8UHxwVJA6zjZZqP8v8kK8OWLnIZtLyCAJagYC4rTGW/9Pqj92N/c+LUaAj27movwbi19tk/whRCIE7Q9vyI6yvRpftAKVTdUjOW40X3h5OXsKCdmFcx0xlLJoSuQngnrJe7Kcjm4OMq9FlC7CMmScQANuNvjfP3PjGXDBaUQmbp296S5L4DrpbrHN1T87ZVEZVCzg1FF0Ft+dKrlLukI+/c9ENo+TvlTDbYFvuKPtQ9+l052rXrgKoWkDAFnvh0wTOmYn8R5f4k/jN/fZiCM1tQx9jQQ4ANhqG4hiL0qIFTGViG9DKB7GYzgubnpofgYRwO+DFjh0Zin2m4b/97EDkXkc+f6xYAPX0KK2I/7fUQuwzuwo/L3AkcjugPNixC8cHf0FyPjWlItmLxWw4Ou9YsQCr5fijMGoD/zpdRy95HRysyXA74MWOnscpO4j2y3HAVisw85hX5+AFBRSHt4ShfLFkIMXTqyKFc46xdzQM6XbAi702a7sy04J0+feReMFKp5q9esYLCqAZYw/k14E/xcLLsFElaornTuJB0svMuJINy8xkIYuL+xPAlWRceH6+HX7THJ0djLUom46zREu7tTkxwmf/FdOZ/sh6Q8qvEAiHpm4PJ4a/doJe0gH1t+aHRgCzOvBvJedEK5OFE5jpm4AGP2a8Dxe3gGJ/pAutug9Gp6he92CsSsWBaEcxGx0FHytmIpuqGkOpldqNYQK8cSoXvd+xLxXADw0kf6UkJNFtdo5MOgaLjiQOQHcn+A6h5NuL2s0qsC2LOM75PcF3yr5STuBSAcGG+meA14K/CI21HcS4LBT6tv0QAh8Dr5l93AhZzG5ZJ4VxAqdZUEl9z7WJ4aN+svMvwHHL21UKTd1mqvChH7/Za5xzXBBKrUcB0TQ+Ulgkfbi/H/YT5EptrGzsEK7tR1B7ln9BBwckYfMiuSqklSznIuoIIOM42MQO+QnduCoFCI0bpkzjCjddHPN/F+2Yu+sd9bKNpVwHhbS3LluK/0zgfwD0xYI5dXuzlQAAAABJRU5ErkJggg==');
 }
 
 div.callout-warning .callout-header {
-  background-color: #fcefdc
+  background-color: #fcefdc;
 }
 
 div.callout-tip {
   border-left-color: #02b875 !important;
 }
 
 div.callout-tip .callout-icon::before {
   background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAADr0lEQVRYCe1XTWgTQRj9ZjZV8a9SPIkKgj8I1bMHsUWrqYLVg4Ue6v9BwZOxSYsIerFao7UiUryIqJcqgtpimhbBXoSCVxUFe9CTiogUrUp2Pt+3aUI2u5vdNh4dmMzOzHvvezuz8xNFM0mjnbXaNu1MvFWRXkXEyE6aYOYJpdW4IXuA4r0fo8qqSMDBU0v1HJUgVieAXxzCsdE/YJTdFcVIZQNMyhruOMJKXYFoLfIfIvVIMWdsrd+Rpd86ZmyzzjJmLStqRn0v8lzkb4rVIXvnpScOJuAn2ACC65FkPzEdEy4TPWRLJ2h7z4cArXzzaOdKlbOvKKX25Wl00jSnrwVxAg3o4dRxhO13RBSdNvH0xSARv3adTXbBdTf64IWO2vH0LT+cv4GR1DJt+DUItaQogeBX/chhbTBxEiZ6gftlDNXTrvT7co4ub5A6gp9HIcHvzTa46OS5fBeP87Qm0fQkr4FsYgVQ7Qg+ZayaDg9jhg1GkWj8RG6lkeSacrrHgDaxdoBiZPg+NXV/KifMuB6//JmYH4CntVEHy/keA6x4h4CU5oFy8GzrBS18cLJMXcljAKB6INjWsRcuZBWVaS3GDrqB7rdapVIeA+isQ57Eev9eCqzqOa81CY05VLd6SamW2wA2H3SiTbnbSxmzfp7WtKZkqy4mdyAlGx7ennghYf8voqp9cLSgKdqNfa6RdRsAAkPwRuJZNbpByn+RrJi1RXTwdi8RQF6ymDwGMAtZ6TVE+4uoKh+MYkcLsT0Hk8eAienbiGdjJHZTpmNjlbFJNKDVAp2fJlYju6IreQxQ08UJDNYdoLSl6AadO+fFuCQqVMB1NJwPm69T04Wv5WhfcWyfXQB+wXRs1pt+nCknRa0LVzSA/2B+a9+zQJadb7IyyV24YAxKp2Jqs3emZTuNnKxsah+uabKbMk7CbTgJx/zIgQYErIeTKRQ9yD9wxVof5YolPHqaWo7TD6tJlh7jQnK5z2n3+fGdggIOx2kaa2YI9QWarc5Ce1ipNWMKeSG4DysFF52KBmTNMmn5HqCFkwy34rDg05gDwgH3bBi+sgFhN/e8QvRn8kbamCOhgrZ9GJhFDgfcMHzFb6BAtjKpFhzTjwv1KCVuxHvCbsSiEz4CANnj84cwHdFXAbAOJ4LTSAawGWFn5tDhLMYz6nWeU2wJfIhmIJBefcd/A5FWQWGgrWzyORZ3Q6HuV+Jf0Bj+BTX69fm1zWgK7By1YTXchFDORywnfQ7GpzOo6S+qECrsx2ifVQAAAABJRU5ErkJggg==');
 }
 
 div.callout-tip .callout-header {
-  background-color: #ccf1e3
+  background-color: #ccf1e3;
 }
 
 div.callout-caution {
   border-left-color: #fd7e14 !important;
 }
 
 div.callout-caution .callout-icon::before {
   background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAIKADAAQAAAABAAAAIAAAAACshmLzAAACV0lEQVRYCdVWzWoUQRCuqp2ICBLJXgITZL1EfQDBW/bkzUMUD7klD+ATSHBEfAIfQO+iXsWDxJsHL96EHAwhgzlkg8nBg25XWb0zIb0zs9muYYWkoKeru+vn664fBqElyZNuyh167NXJ8Ut8McjbmEraKHkd7uAnAFku+VWdb3reSmRV8PKSLfZ0Gjn3a6Xlcq9YGb6tADjn+lUfTXtVmaZ1KwBIvFI11rRXlWlatwIAAv2asaa9mlB9wwygiDX26qaw1yYPzFXg2N1GgG0FMF8Oj+VIx7E/03lHx8UhvYyNZLN7BwSPgekXXLribw7w5/c8EF+DBK5idvDVYtEEwMeYefjjLAdEyQ3M9nfOkgnPTEkYU+sxMq0BxNR6jExrAI31H1rzvLEfRIdgcv1XEdj6QTQAS2wtstEALLG1yEZ3QhH6oDX7ExBSFEkFINXH98NTrme5IOaaA7kIfiu2L8A3qhH9zRbukdCqdsA98TdElyeMe5BI8Rs2xHRIsoTSSVFfCFCWGPn9XHb4cdobRIWABNf0add9jakDjQJpJ1bTXOJXnnRXHRf+dNL1ZV1MBRCXhMbaHqGI1JkKIL7+i8uffuP6wVQAzO7+qVEbF6NbS0LJureYcWXUUhH66nLR5rYmva+2tjRFtojkM2aD76HEGAD3tPtKM309FJg5j/K682ywcWJ3PASCcycH/22u+Bh7Aa0ehM2Fu4z0SAE81HF9RkB21c5bEn4Dzw+/qNOyXr3DCTQDMBOdhi4nAgiFDGCinIa2owCEChUwD8qzd03PG+qdW/4fDzjUMcE1ZpIAAAAASUVORK5CYII=');
 }
 
 div.callout-caution .callout-header {
-  background-color: #ffe5d0
+  background-color: #ffe5d0;
+}
+
+.callout.callout-style-default .callout-icon::before {
+  height: 1rem;
+  width: 1rem;
+  display: inline-block;
+  content: '';
+  background-repeat: no-repeat;
+  background-size: 1rem 1rem;
+  margin-bottom: -3px;
+  padding-right: 0.4rem;
 }
 
 /* Shortcodes */
 
 span.shortcode {
   font-family: var(--jp-code-font-family);
   line-height: var(--jp-code-line-height);
   color: var(--jp-content-link-color);
   background-color: var(--jp-layout-color2);
-  padding: 1px 1px;
+  padding: 1px;
   white-space: pre-wrap;
 }
```

### Comparing `jupyterlab_quarto-0.1.45/LICENSE` & `jupyterlab_quarto-0.2.2/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Posit, PBC
+Copyright (c) 2023, Charles Teague
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `jupyterlab_quarto-0.1.45/README.md` & `jupyterlab_quarto-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,112 @@
 # JupyterLab Quarto Extension
 
-[Quarto](https://www.quarto.org) is an open source project that combines Jupyter notebooks with flexible options to use a single source document to produce high-quality articles, reports, presentations, websites, and books in HTML, PDF, MS Word, ePub, and more. Quarto supports a wide variety of useful new features useful in technical documents, including support for LaTeX equations, citations, cross-references, figure panels, callouts, advanced page layout, and more. 
+[Quarto](https://www.quarto.org) is an open source project that combines Jupyter notebooks with flexible options to use a single source document to produce high-quality articles, reports, presentations, websites, and books in HTML, PDF, MS Word, ePub, and more. Quarto supports a wide variety of useful new features useful in technical documents, including support for LaTeX equations, citations, cross-references, figure panels, callouts, advanced page layout, and more.
 
 The JupyterLab Quarto extension allows JupyterLab to render notebooks which include Quarto markdown content.
 <br/><br/>
+
 <p align="center">
 <img src="https://user-images.githubusercontent.com/261654/230087634-d5027ebc-8508-43b4-81c9-c4b7d6cfa738.png" width="60%">
 </p>
 
+### Binder
+
+You can try an example of the extension in a notebook (though you can't actually render the notebook using Quarto) on Binder.
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/quarto-dev/jupyterlab-quarto/main?urlpath=lab)
+
+## Status
+
+[![Github Actions Status](https://github.com/quarto-dev/jupyterlab-quarto/workflows/Build/badge.svg)](https://github.com/quarto-dev/jupyterlab-quarto/actions/workflows/build.yml)
+
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlab-quarto
+pip install jupyterlab_quarto
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall jupyterlab-quarto
+pip uninstall jupyterlab_quarto
 ```
 
 ## Contributing
 
 ### Development install
 
+Note: You will need NodeJS to build the extension package.
+
+The `jlpm` command is JupyterLab's pinned version of
+[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
+`yarn` or `npm` in lieu of `jlpm` below.
+
 ```bash
-# From apps/jupyterlab
+# Clone the repo to your local environment
+# Change directory to the jupyterlab_quarto directory
 # Install package in development mode
 pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
-yarn build
+jlpm build
 ```
-Note: You will need NodeJS to build the extension package.
-
-Note: The `jlpm` command is JupyterLab's pinned version of
-[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
-`yarn` or `npm` in lieu of `jlpm` below.
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
-yarn watch
+jlpm watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
-By default, the `build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
+By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-pip uninstall jupyterlab-quarto
+pip uninstall jupyterlab_quarto
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `jupyterlab-quarto` within that folder.
+folder is located. Then you can remove the symlink named `jupyterlab_quarto` within that folder.
+
+### Testing the extension
+
+#### Frontend tests
+
+This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
+
+To execute them, execute:
+
+```sh
+jlpm
+jlpm test
+```
+
+#### Integration tests
+
+This extension uses [Playwright](https://playwright.dev/) for the integration tests (aka user level tests).
+More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
+
+More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

### Comparing `jupyterlab_quarto-0.1.45/pyproject.toml` & `jupyterlab_quarto-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
-requires = ["hatchling>=1.4.0", "jupyterlab>=3.4.7,<4.0.0", "hatch-nodejs-version"]
+requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
-name = "jupyterlab-quarto"
+name = "jupyterlab_quarto"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
-    "Framework :: Jupyter :: JupyterLab :: 3",
+    "Framework :: Jupyter :: JupyterLab :: 4",
     "Framework :: Jupyter :: JupyterLab :: Extensions",
     "Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
 ]
@@ -29,45 +28,49 @@
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
-artifacts = ["jupyterlab-quarto/labextension"]
+artifacts = ["jupyterlab_quarto/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
-"jupyterlab-quarto/labextension" = "share/jupyter/labextensions/jupyterlab-quarto"
-"install.json" = "share/jupyter/labextensions/jupyterlab-quarto/install.json"
+"jupyterlab_quarto/labextension" = "share/jupyter/labextensions/jupyterlab_quarto"
+"install.json" = "share/jupyter/labextensions/jupyterlab_quarto/install.json"
 
 [tool.hatch.build.hooks.version]
-path = "jupyterlab-quarto/_version.py"
+path = "jupyterlab_quarto/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
-    "jupyterlab-quarto/labextension/static/style.js",
-    "jupyterlab-quarto/labextension/package.json",
+    "jupyterlab_quarto/labextension/static/style.js",
+    "jupyterlab_quarto/labextension/package.json",
 ]
-skip-if-exists = ["jupyterlab-quarto/labextension/static/style.js"]
+skip-if-exists = ["jupyterlab_quarto/labextension/static/style.js"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 build_cmd = "build:prod"
 npm = ["jlpm"]
 
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
-build_dir = "jupyterlab-quarto/labextension"
+build_dir = "jupyterlab_quarto/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
-before-build-npm = ["python -m pip install jupyterlab~=3.1", "jlpm", "jlpm build:prod"]
+before-build-npm = [
+    "python -m pip install 'jupyterlab>=4.0.0,<5'",
+    "jlpm",
+    "jlpm build:prod"
+]
 before-build-python = ["jlpm clean:all"]
 
 [tool.check-wheel-contents]
 ignore = ["W002"]
```

### Comparing `jupyterlab_quarto-0.1.45/PKG-INFO` & `jupyterlab_quarto-0.2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
-Name: jupyterlab-quarto
-Version: 0.1.45
+Name: jupyterlab_quarto
+Version: 0.2.2
 Summary: Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.
-Project-URL: Homepage, https://github.com/quarto-dev/quarto
-Project-URL: Bug Tracker, https://github.com/quarto-dev/quarto/issues/
-Project-URL: Repository, https://github.com/quarto-dev/quarto/quarto.git
+Project-URL: Homepage, https://github.com/quarto-dev/jupyterlab-quarto
+Project-URL: Bug Tracker, https://github.com/quarto-dev/jupyterlab-quarto/issues
+Project-URL: Repository, https://github.com/quarto-dev/jupyterlab-quarto.git
 Author-email: Charles Teague <charles@posit.co>
 License: BSD 3-Clause License
         
-        Copyright (c) 2023, Posit, PBC
+        Copyright (c) 2023, Charles Teague
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -34,100 +34,132 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # JupyterLab Quarto Extension
 
-[Quarto](https://www.quarto.org) is an open source project that combines Jupyter notebooks with flexible options to use a single source document to produce high-quality articles, reports, presentations, websites, and books in HTML, PDF, MS Word, ePub, and more. Quarto supports a wide variety of useful new features useful in technical documents, including support for LaTeX equations, citations, cross-references, figure panels, callouts, advanced page layout, and more. 
+[Quarto](https://www.quarto.org) is an open source project that combines Jupyter notebooks with flexible options to use a single source document to produce high-quality articles, reports, presentations, websites, and books in HTML, PDF, MS Word, ePub, and more. Quarto supports a wide variety of useful new features useful in technical documents, including support for LaTeX equations, citations, cross-references, figure panels, callouts, advanced page layout, and more.
 
 The JupyterLab Quarto extension allows JupyterLab to render notebooks which include Quarto markdown content.
 <br/><br/>
+
 <p align="center">
 <img src="https://user-images.githubusercontent.com/261654/230087634-d5027ebc-8508-43b4-81c9-c4b7d6cfa738.png" width="60%">
 </p>
 
+### Binder
+
+You can try an example of the extension in a notebook (though you can't actually render the notebook using Quarto) on Binder.
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/quarto-dev/jupyterlab-quarto/main?urlpath=lab)
+
+## Status
+
+[![Github Actions Status](https://github.com/quarto-dev/jupyterlab-quarto/workflows/Build/badge.svg)](https://github.com/quarto-dev/jupyterlab-quarto/actions/workflows/build.yml)
+
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlab-quarto
+pip install jupyterlab_quarto
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall jupyterlab-quarto
+pip uninstall jupyterlab_quarto
 ```
 
 ## Contributing
 
 ### Development install
 
+Note: You will need NodeJS to build the extension package.
+
+The `jlpm` command is JupyterLab's pinned version of
+[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
+`yarn` or `npm` in lieu of `jlpm` below.
+
 ```bash
-# From apps/jupyterlab
+# Clone the repo to your local environment
+# Change directory to the jupyterlab_quarto directory
 # Install package in development mode
 pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
-yarn build
+jlpm build
 ```
-Note: You will need NodeJS to build the extension package.
-
-Note: The `jlpm` command is JupyterLab's pinned version of
-[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
-`yarn` or `npm` in lieu of `jlpm` below.
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
-yarn watch
+jlpm watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
-By default, the `build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
+By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
 
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-pip uninstall jupyterlab-quarto
+pip uninstall jupyterlab_quarto
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `jupyterlab-quarto` within that folder.
+folder is located. Then you can remove the symlink named `jupyterlab_quarto` within that folder.
+
+### Testing the extension
+
+#### Frontend tests
+
+This extension is using [Jest](https://jestjs.io/) for JavaScript code testing.
+
+To execute them, execute:
+
+```sh
+jlpm
+jlpm test
+```
+
+#### Integration tests
+
+This extension uses [Playwright](https://playwright.dev/) for the integration tests (aka user level tests).
+More precisely, the JupyterLab helper [Galata](https://github.com/jupyterlab/jupyterlab/tree/master/galata) is used to handle testing the extension in JupyterLab.
+
+More information are provided within the [ui-tests](./ui-tests/README.md) README.
 
 ### Packaging the extension
 
 See [RELEASE](RELEASE.md)
```

