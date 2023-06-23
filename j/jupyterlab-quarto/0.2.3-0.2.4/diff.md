# Comparing `tmp/jupyterlab_quarto-0.2.3.tar.gz` & `tmp/jupyterlab_quarto-0.2.4.tar.gz`

## Comparing `jupyterlab_quarto-0.2.3.tar` & `jupyterlab_quarto-0.2.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/.copier-answers.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/.yarnrc.yml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jest.config.js
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/tsconfig.test.json
--rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/yarn.lock
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/_version.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/package.json
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/11.bbf21e9c517bec162b9c.js
--rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
--rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/150.9b2f6283ffc934651e1c.js
--rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/185.a8ca3522cb5c31423453.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
--rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/316.f7e4dd762f98107da4a5.js
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/384.6c76694e25edf7010d50.js
--rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/487.dee02fd512e9bb15dee6.js
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/543.40a7a1799fcad108039e.js
--rw-r--r--   0        0        0    42379 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/573.79885c9e9fcb552239cd.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/573.79885c9e9fcb552239cd.js.LICENSE.txt
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/596.ef22233afe464ab9134a.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/645.406375856388e9d7e4e9.js
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/651.7673e27b3217024cb32d.js
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/700.30097f2c1808e10c985f.js
--rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/724.265325864c2c7d67e29e.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
--rw-r--r--   0        0        0    28859 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/923.b51eb181f4c017b19c97.js
--rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/980.57fcdfda225b581383c0.js
--rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/remoteEntry.af54ba43087a3a104368.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/style.js
--rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/const.ts
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/index.ts
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/manager.ts
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/types.ts
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/widgets.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-deflist.d.ts
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-footnote.d.ts
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-gridtables.d.ts
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-implicit-figures.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-sub.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-sup.d.ts
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/@types/markdown-it-task-lists.d.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/__tests__/jupyterlab_quarto.spec.ts
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/ast/ast.ts
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/hooks/codemirror.ts
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/callouts.ts
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/cites.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/decorator.ts
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/divs.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/figure-divs.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/figures.ts
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/index.ts
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/math.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/shortcodes.ts
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/spans.ts
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/table-captions.ts
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/yaml.ts
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/index.ts
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/gridtables/GetCells.ts
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/EmitTable.ts
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/GetLine.ts
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/ParseTable.ts
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/interfaces/markdown-it/IState.ts
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/gridtables/rules/gridtable.ts
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/mermaid/index.ts
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/utils/html.ts
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/utils/markdownit.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/plugins/utils/tok.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/attrs.ts
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/callouts.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/cites.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/decorator.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/deflist.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/divs.ts
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/figure-divs.ts
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/figures.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/footnotes.ts
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/gridtables.ts
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/math.ts
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/mermaid.ts
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/provider.ts
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/shortcodes.ts
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/spans.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/sub.ts
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/sup.ts
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/table-captions.ts
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/tasklists.ts
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/src/providers/yaml.ts
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/ui-tests/tests/jupyterlab_quarto.spec.ts
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/LICENSE
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/README.md
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/.copier-answers.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/.yarnrc.yml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jest.config.js
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/tsconfig.test.json
+-rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/yarn.lock
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/_version.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/package.json
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js
+-rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js
+-rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
+-rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js
+-rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js
+-rw-r--r--   0        0        0    42379 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js.LICENSE.txt
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js
+-rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
+-rw-r--r--   0        0        0    28859 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/remoteEntry.3acb7e5c1bb3e29649b3.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/style.js
+-rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/const.ts
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/index.ts
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/manager.ts
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/types.ts
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/widgets.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-deflist.d.ts
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-footnote.d.ts
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-gridtables.d.ts
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-implicit-figures.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-sub.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-sup.d.ts
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/@types/markdown-it-task-lists.d.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/__tests__/jupyterlab-quarto.spec.ts
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/ast/ast.ts
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/hooks/codemirror.ts
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/callouts.ts
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/cites.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/decorator.ts
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/divs.ts
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/figure-divs.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/figures.ts
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/index.ts
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/math.ts
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/shortcodes.ts
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/spans.ts
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/table-captions.ts
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/yaml.ts
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/index.ts
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/gridtables/GetCells.ts
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/EmitTable.ts
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/GetLine.ts
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/ParseTable.ts
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/interfaces/markdown-it/IState.ts
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/gridtables/rules/gridtable.ts
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/mermaid/index.ts
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/utils/html.ts
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/utils/markdownit.ts
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/plugins/utils/tok.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/attrs.ts
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/callouts.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/cites.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/decorator.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/deflist.ts
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/divs.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/figure-divs.ts
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/figures.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/footnotes.ts
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/gridtables.ts
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/math.ts
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/mermaid.ts
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/provider.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/shortcodes.ts
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/spans.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/sub.ts
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/sup.ts
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/table-captions.ts
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/tasklists.ts
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/src/providers/yaml.ts
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/ui-tests/tests/jupyterlab-quarto.spec.ts
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/README.md
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.4/PKG-INFO
```

### Comparing `jupyterlab_quarto-0.2.3/.copier-answers.yml` & `jupyterlab_quarto-0.2.4/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/RELEASE.md` & `jupyterlab_quarto-0.2.4/RELEASE.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Making a new release of jupyterlab_quarto
+# Making a new release of jupyterlab-quarto
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
 ### Python package
 
@@ -24,28 +24,21 @@
 **Before building, note that you must temporarily update the `package.json` file to remove the `@quarto` prefix from the package name.**
 
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 ```bash
 jlpm clean:all
 git clean -dfX
-rm dist/*
 jlpm build
 python -m build
 twine upload dist/*
 ```
 
 > `python setup.py sdist bdist_wheel` is deprecated and will not work for this package.
 
-Then to upload the package to PyPI, do:
-
-```bash
-
-```
-
 ### NPM package
 
 To publish the frontend part of the extension as a NPM package, do:
 
 ```bash
 jlpm clean:all
 git clean -dfX
```

### Comparing `jupyterlab_quarto-0.2.3/jest.config.js` & `jupyterlab_quarto-0.2.4/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/package.json` & `jupyterlab_quarto-0.2.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9752777777777779%*

 * *Differences: {"'jupyterlab'": "{'outputDir': 'jupyterlab-quarto/labextension'}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf jupyterlab-quarto/labextension "*

 * *              "jupyterlab-quarto/_version.py'}",*

 * * "'version'": "'0.2.4'"}*

```diff
@@ -113,15 +113,15 @@
     "jupyterlab": {
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
         "extension": true,
-        "outputDir": "jupyterlab_quarto/labextension"
+        "outputDir": "jupyterlab-quarto/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -145,15 +145,15 @@
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_quarto/labextension jupyterlab_quarto/_version.py",
+        "clean:labextension": "rimraf jupyterlab-quarto/labextension jupyterlab-quarto/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.2.4"
 }
```

### Comparing `jupyterlab_quarto-0.2.3/tsconfig.json` & `jupyterlab_quarto-0.2.4/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/yarn.lock` & `jupyterlab_quarto-0.2.4/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/__init__.py` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from ._version import __version__
 except ImportError:
     # Fallback when using the package in dev mode without installing
     # in editable mode with pip. It is highly recommended to install
     # the package from a stable release or in editable mode: https://pip.pypa.io/en/stable/topics/local-project-installs/#editable-installs
     import warnings
-    warnings.warn("Importing 'jupyterlab_quarto' outside a proper installation.")
+    warnings.warn("Importing 'jupyterlab-quarto' outside a proper installation.")
     __version__ = "dev"
 
 
 def _jupyter_labextension_paths():
     return [{
         "src": "labextension",
         "dest": "@quarto/jupyterlab-quarto"
```

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/package.json` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9757118055555556%*

 * *Differences: {"'jupyterlab'": "{'outputDir': 'jupyterlab-quarto/labextension', '_build': {'load': "*

 * *                 "'static/remoteEntry.3acb7e5c1bb3e29649b3.js'}}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf jupyterlab-quarto/labextension "*

 * *              "jupyterlab-quarto/_version.py'}",*

 * * "'version'": "'0.2.4'"}*

```diff
@@ -109,24 +109,24 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/quarto-dev/jupyterlab-quarto",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.af54ba43087a3a104368.js",
+            "load": "static/remoteEntry.3acb7e5c1bb3e29649b3.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
         "extension": true,
-        "outputDir": "jupyterlab_quarto/labextension"
+        "outputDir": "jupyterlab-quarto/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -150,15 +150,15 @@
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf jupyterlab_quarto/labextension jupyterlab_quarto/_version.py",
+        "clean:labextension": "rimraf jupyterlab-quarto/labextension jupyterlab-quarto/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -188,9 +188,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.3"
+    "version": "0.2.4"
 }
```

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/11.bbf21e9c517bec162b9c.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/136.43b409c7c7e6885bc7ee.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/150.9b2f6283ffc934651e1c.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/185.a8ca3522cb5c31423453.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/316.f7e4dd762f98107da4a5.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/384.6c76694e25edf7010d50.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/487.dee02fd512e9bb15dee6.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/543.40a7a1799fcad108039e.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/573.79885c9e9fcb552239cd.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/596.ef22233afe464ab9134a.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/645.406375856388e9d7e4e9.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/651.7673e27b3217024cb32d.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/700.30097f2c1808e10c985f.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/724.265325864c2c7d67e29e.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/923.b51eb181f4c017b19c97.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/980.57fcdfda225b581383c0.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/remoteEntry.af54ba43087a3a104368.js` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/remoteEntry.3acb7e5c1bb3e29649b3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -168,15 +168,15 @@
                         (!f || !f.loaded && (!a != !f.eager ? a : d > f.from)) && (n[t] = {
                             get: r,
                             from: d,
                             eager: !!a
                         })
                     },
                     i = [];
-                return "default" === r && (f("jupyterlab-quarto", "0.2.3", (() => Promise.all([P.e(185), P.e(573), P.e(150), P.e(923)]).then((() => () => P(5923))))), f("markdown-it-attrs", "4.1.6", (() => P.e(543).then((() => () => P(9543))))), f("markdown-it-deflist", "2.1.0", (() => P.e(645).then((() => () => P(645))))), f("markdown-it-footnote", "3.0.3", (() => P.e(384).then((() => () => P(2384))))), f("markdown-it-sub", "1.0.0", (() => P.e(700).then((() => () => P(700))))), f("markdown-it-sup", "1.0.0", (() => P.e(3).then((() => () => P(7003))))), f("markdown-it-task-lists", "1.4.1", (() => P.e(651).then((() => () => P(4651))))), f("markdown-it", "12.3.2", (() => Promise.all([P.e(980), P.e(185)]).then((() => () => P(9980))))), f("mermaid", "9.4.3", (() => P.e(136).then((() => () => P(4136))))), f("wcwidth", "1.0.1", (() => P.e(11).then((() => () => P(1011)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
+                return "default" === r && (f("jupyterlab-quarto", "0.2.4", (() => Promise.all([P.e(185), P.e(573), P.e(150), P.e(923)]).then((() => () => P(5923))))), f("markdown-it-attrs", "4.1.6", (() => P.e(543).then((() => () => P(9543))))), f("markdown-it-deflist", "2.1.0", (() => P.e(645).then((() => () => P(645))))), f("markdown-it-footnote", "3.0.3", (() => P.e(384).then((() => () => P(2384))))), f("markdown-it-sub", "1.0.0", (() => P.e(700).then((() => () => P(700))))), f("markdown-it-sup", "1.0.0", (() => P.e(3).then((() => () => P(7003))))), f("markdown-it-task-lists", "1.4.1", (() => P.e(651).then((() => () => P(4651))))), f("markdown-it", "12.3.2", (() => Promise.all([P.e(980), P.e(185)]).then((() => () => P(9980))))), f("mermaid", "9.4.3", (() => P.e(136).then((() => () => P(4136))))), f("wcwidth", "1.0.1", (() => P.e(11).then((() => () => P(1011)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var t = P.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
```

### Comparing `jupyterlab_quarto-0.2.3/jupyterlab_quarto/labextension/static/third-party-licenses.json` & `jupyterlab_quarto-0.2.4/jupyterlab-quarto/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/index.ts` & `jupyterlab_quarto-0.2.4/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/manager.ts` & `jupyterlab_quarto-0.2.4/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/types.ts` & `jupyterlab_quarto-0.2.4/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/widgets.ts` & `jupyterlab_quarto-0.2.4/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/ast/ast.ts` & `jupyterlab_quarto-0.2.4/src/ast/ast.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/hooks/codemirror.ts` & `jupyterlab_quarto-0.2.4/src/hooks/codemirror.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/callouts.ts` & `jupyterlab_quarto-0.2.4/src/plugins/callouts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/cites.ts` & `jupyterlab_quarto-0.2.4/src/plugins/cites.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/decorator.ts` & `jupyterlab_quarto-0.2.4/src/plugins/decorator.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/divs.ts` & `jupyterlab_quarto-0.2.4/src/plugins/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/figure-divs.ts` & `jupyterlab_quarto-0.2.4/src/plugins/figure-divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/figures.ts` & `jupyterlab_quarto-0.2.4/src/plugins/figures.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/index.ts` & `jupyterlab_quarto-0.2.4/src/plugins/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/math.ts` & `jupyterlab_quarto-0.2.4/src/plugins/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/shortcodes.ts` & `jupyterlab_quarto-0.2.4/src/plugins/shortcodes.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/spans.ts` & `jupyterlab_quarto-0.2.4/src/plugins/spans.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/table-captions.ts` & `jupyterlab_quarto-0.2.4/src/plugins/table-captions.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/yaml.ts` & `jupyterlab_quarto-0.2.4/src/plugins/yaml.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/index.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/gridtables/GetCells.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/gridtables/GetCells.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/EmitTable.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/EmitTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/GetLine.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/GetLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/ParseTable.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/ParseTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/interfaces/markdown-it/IState.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/interfaces/markdown-it/IState.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/gridtables/rules/gridtable.ts` & `jupyterlab_quarto-0.2.4/src/plugins/gridtables/rules/gridtable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/mermaid/index.ts` & `jupyterlab_quarto-0.2.4/src/plugins/mermaid/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/utils/html.ts` & `jupyterlab_quarto-0.2.4/src/plugins/utils/html.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/plugins/utils/markdownit.ts` & `jupyterlab_quarto-0.2.4/src/plugins/utils/markdownit.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/providers/divs.ts` & `jupyterlab_quarto-0.2.4/src/providers/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/providers/math.ts` & `jupyterlab_quarto-0.2.4/src/providers/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/src/providers/provider.ts` & `jupyterlab_quarto-0.2.4/src/providers/provider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/style/base.css` & `jupyterlab_quarto-0.2.4/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/ui-tests/README.md` & `jupyterlab_quarto-0.2.4/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/ui-tests/tests/jupyterlab_quarto.spec.ts` & `jupyterlab_quarto-0.2.4/ui-tests/tests/jupyterlab-quarto.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/.gitignore` & `jupyterlab_quarto-0.2.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 node_modules/
 *.log
 .eslintcache
 .stylelintcache
 *.egg-info/
 .ipynb_checkpoints
 *.tsbuildinfo
-jupyterlab_quarto/labextension
+jupyterlab-quarto/labextension
 # Version file is handled by hatchling
-jupyterlab_quarto/_version.py
+jupyterlab-quarto/_version.py
 
 # Integration tests
 ui-tests/test-results/
 ui-tests/playwright-report/
 
 # Created by https://www.gitignore.io/api/python
 # Edit at https://www.gitignore.io/?templates=python
```

### Comparing `jupyterlab_quarto-0.2.3/LICENSE` & `jupyterlab_quarto-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.3/README.md` & `jupyterlab_quarto-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,38 +24,38 @@
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlab_quarto
+pip install jupyterlab-quarto
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall jupyterlab_quarto
+pip uninstall jupyterlab-quarto
 ```
 
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Change directory to the jupyterlab_quarto directory
+# Change directory to the jupyterlab-quarto directory
 # Install package in development mode
 pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
@@ -76,15 +76,15 @@
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-pip uninstall jupyterlab_quarto
+pip uninstall jupyterlab-quarto
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `@quarto/jupyterlab-quarto` within that folder.
 
 ### Testing the extension
```

### Comparing `jupyterlab_quarto-0.2.3/pyproject.toml` & `jupyterlab_quarto-0.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling>=1.5.0", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version"]
 build-backend = "hatchling.build"
 
 [project]
-name = "jupyterlab_quarto"
+name = "jupyterlab-quarto"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 4",
@@ -28,42 +28,42 @@
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
-artifacts = ["jupyterlab_quarto/labextension"]
+artifacts = ["jupyterlab-quarto/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
-"jupyterlab_quarto/labextension" = "share/jupyter/labextensions/@quarto/jupyterlab-quarto"
+"jupyterlab-quarto/labextension" = "share/jupyter/labextensions/@quarto/jupyterlab-quarto"
 "install.json" = "share/jupyter/labextensions/@quarto/jupyterlab-quarto/install.json"
 
 [tool.hatch.build.hooks.version]
-path = "jupyterlab_quarto/_version.py"
+path = "jupyterlab-quarto/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
-    "jupyterlab_quarto/labextension/static/style.js",
-    "jupyterlab_quarto/labextension/package.json",
+    "jupyterlab-quarto/labextension/static/style.js",
+    "jupyterlab-quarto/labextension/package.json",
 ]
-skip-if-exists = ["jupyterlab_quarto/labextension/static/style.js"]
+skip-if-exists = ["jupyterlab-quarto/labextension/static/style.js"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 build_cmd = "build:prod"
 npm = ["jlpm"]
 
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
-build_dir = "jupyterlab_quarto/labextension"
+build_dir = "jupyterlab-quarto/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
 before-build-npm = [
     "python -m pip install 'jupyterlab>=4.0.0,<5'",
```

### Comparing `jupyterlab_quarto-0.2.3/PKG-INFO` & `jupyterlab_quarto-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jupyterlab_quarto
-Version: 0.2.3
+Name: jupyterlab-quarto
+Version: 0.2.4
 Summary: Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.
 Project-URL: Homepage, https://github.com/quarto-dev/jupyterlab-quarto
 Project-URL: Bug Tracker, https://github.com/quarto-dev/jupyterlab-quarto/issues
 Project-URL: Repository, https://github.com/quarto-dev/jupyterlab-quarto.git
 Author-email: Charles Teague <charles@posit.co>
 License: BSD 3-Clause License
         
@@ -77,38 +77,38 @@
 - JupyterLab >= 4.0.0
 
 ## Install
 
 To install the extension, execute:
 
 ```bash
-pip install jupyterlab_quarto
+pip install jupyterlab-quarto
 ```
 
 ## Uninstall
 
 To remove the extension, execute:
 
 ```bash
-pip uninstall jupyterlab_quarto
+pip uninstall jupyterlab-quarto
 ```
 
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
 The `jlpm` command is JupyterLab's pinned version of
 [yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
 `yarn` or `npm` in lieu of `jlpm` below.
 
 ```bash
 # Clone the repo to your local environment
-# Change directory to the jupyterlab_quarto directory
+# Change directory to the jupyterlab-quarto directory
 # Install package in development mode
 pip install -e "."
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
 jlpm build
 ```
@@ -129,15 +129,15 @@
 ```bash
 jupyter lab build --minimize=False
 ```
 
 ### Development uninstall
 
 ```bash
-pip uninstall jupyterlab_quarto
+pip uninstall jupyterlab-quarto
 ```
 
 In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `@quarto/jupyterlab-quarto` within that folder.
 
 ### Testing the extension
```

