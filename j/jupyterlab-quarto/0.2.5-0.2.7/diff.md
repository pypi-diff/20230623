# Comparing `tmp/jupyterlab_quarto-0.2.5.tar.gz` & `tmp/jupyterlab_quarto-0.2.7.tar.gz`

## Comparing `jupyterlab_quarto-0.2.5.tar` & `jupyterlab_quarto-0.2.7.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/.copier-answers.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/.yarnrc.yml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/CHANGELOG.md
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/babel.config.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jest.config.js
--rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/setup.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/tsconfig.test.json
--rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/yarn.lock
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/_version.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/package.json
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js
--rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
--rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js
--rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
--rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js
--rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js
--rw-r--r--   0        0        0    42379 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js.LICENSE.txt
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js
--rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
--rw-r--r--   0        0        0    28859 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js
--rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js
--rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/remoteEntry.ee954710581352bf9b27.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/style.js
--rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/const.ts
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/index.ts
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/manager.ts
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/types.ts
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/widgets.ts
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-deflist.d.ts
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-footnote.d.ts
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-gridtables.d.ts
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-implicit-figures.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-sub.d.ts
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-sup.d.ts
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/@types/markdown-it-task-lists.d.ts
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/__tests__/jupyterlab-quarto.spec.ts
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/ast/ast.ts
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/hooks/codemirror.ts
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/callouts.ts
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/cites.ts
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/decorator.ts
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/divs.ts
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/figure-divs.ts
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/figures.ts
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/index.ts
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/math.ts
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/shortcodes.ts
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/spans.ts
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/table-captions.ts
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/yaml.ts
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/index.ts
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/gridtables/GetCells.ts
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/EmitTable.ts
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/GetLine.ts
--rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/ParseTable.ts
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/interfaces/markdown-it/IState.ts
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/gridtables/rules/gridtable.ts
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/mermaid/index.ts
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/utils/html.ts
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/utils/markdownit.ts
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/plugins/utils/tok.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/attrs.ts
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/callouts.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/cites.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/decorator.ts
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/deflist.ts
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/divs.ts
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/figure-divs.ts
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/figures.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/footnotes.ts
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/gridtables.ts
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/math.ts
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/mermaid.ts
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/provider.ts
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/shortcodes.ts
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/spans.ts
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/sub.ts
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/sup.ts
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/table-captions.ts
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/tasklists.ts
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/src/providers/yaml.ts
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/ui-tests/yarn.lock
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/ui-tests/tests/jupyterlab-quarto.spec.ts
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/LICENSE
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/README.md
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.copier-answers.yml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.yarnrc.yml
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/babel.config.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jest.config.js
+-rw-r--r--   0        0        0     6632 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/setup.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/tsconfig.test.json
+-rw-r--r--   0        0        0   414691 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/yarn.lock
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/_version.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/package.json
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js
+-rw-r--r--   0        0        0   854820 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js.LICENSE.txt
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js
+-rw-r--r--   0        0        0    43658 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js
+-rw-r--r--   0        0        0    19391 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js
+-rw-r--r--   0        0        0  1402360 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js
+-rw-r--r--   0        0        0    42379 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js.LICENSE.txt
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js
+-rw-r--r--   0        0        0   456694 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js.LICENSE.txt
+-rw-r--r--   0        0        0    28859 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/remoteEntry.110f607f4dd53733e5a3.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/style.js
+-rw-r--r--   0        0        0    88824 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/const.ts
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/index.ts
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/manager.ts
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/types.ts
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/widgets.ts
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-deflist.d.ts
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-footnote.d.ts
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-gridtables.d.ts
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-implicit-figures.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-sub.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-sup.d.ts
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/@types/markdown-it-task-lists.d.ts
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/__tests__/jupyterlab-quarto.spec.ts
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/ast/ast.ts
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/hooks/codemirror.ts
+-rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/callouts.ts
+-rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/cites.ts
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/decorator.ts
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/divs.ts
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/figure-divs.ts
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/figures.ts
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/index.ts
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/math.ts
+-rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/shortcodes.ts
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/spans.ts
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/table-captions.ts
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/yaml.ts
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/index.ts
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetCells.ts
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ColumnAlignments.ts
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/EmitTable.ts
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetLine.ts
+-rw-r--r--   0        0        0     5619 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTable.ts
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/IState.ts
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/IToken.ts
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/gridtables/rules/gridtable.ts
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/mermaid/index.ts
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/utils/html.ts
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/utils/markdownit.ts
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/plugins/utils/tok.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/attrs.ts
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/callouts.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/cites.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/decorator.ts
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/deflist.ts
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/divs.ts
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/figure-divs.ts
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/figures.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/footnotes.ts
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/gridtables.ts
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/math.ts
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/mermaid.ts
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/provider.ts
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/shortcodes.ts
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/spans.ts
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/sub.ts
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/sup.ts
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/table-captions.ts
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/tasklists.ts
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/src/providers/yaml.ts
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/ui-tests/tests/jupyterlab-quarto.spec.ts
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/README.md
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 jupyterlab_quarto-0.2.7/PKG-INFO
```

### Comparing `jupyterlab_quarto-0.2.5/.copier-answers.yml` & `jupyterlab_quarto-0.2.7/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/RELEASE.md` & `jupyterlab_quarto-0.2.7/RELEASE.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Making a new release of jupyterlab-quarto
+# Making a new release of jupyterlab_quarto
 
 The extension can be published to `PyPI` and `npm` manually or using the [Jupyter Releaser](https://github.com/jupyter-server/jupyter_releaser).
 
 ## Manual release
 
 ### Python package
 
@@ -22,27 +22,28 @@
 ```
 
 **Before building, note that you must temporarily update the `package.json` file to remove the `@quarto` prefix from the package name.**
 
 To create a Python source package (`.tar.gz`) and the binary package (`.whl`) in the `dist/` directory, do:
 
 ```bash
-jlpm clean:all
-git clean -dfX
-jlpm build
+jlpm clean:all && git clean -dfX
+sed -i '' 's/"@quarto\/jupyterlab-quarto"/"jupyterlab-quarto"/g' package.json
+jlpm && jlpm build:prod
 python -m build
 twine upload dist/*
+sed -i '' 's/"jupyterlab-quarto"/"@quarto\/jupyterlab-quarto"/g' package.json
+jlpm
 ```
 
 > `python setup.py sdist bdist_wheel` is deprecated and will not work for this package.
 
 ### NPM package
 
 To publish the frontend part of the extension as a NPM package, do:
 
 ```bash
-jlpm clean:all
-git clean -dfX
-jlpm build
+jlpm clean:all && git clean -dfX
+jlpm && jlpm build:prod
 npm login
 npm publish --access public
 ```
```

### Comparing `jupyterlab_quarto-0.2.5/jest.config.js` & `jupyterlab_quarto-0.2.7/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/package.json` & `jupyterlab_quarto-0.2.7/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.7'"}*

```diff
@@ -183,9 +183,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.5"
+    "version": "0.2.7"
 }
```

### Comparing `jupyterlab_quarto-0.2.5/tsconfig.json` & `jupyterlab_quarto-0.2.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/yarn.lock` & `jupyterlab_quarto-0.2.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/__init__.py` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/package.json` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.110f607f4dd53733e5a3.js'}}",*

 * * "'version'": "'0.2.7'"}*

```diff
@@ -109,15 +109,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/quarto-dev/jupyterlab-quarto",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ee954710581352bf9b27.js",
+            "load": "static/remoteEntry.110f607f4dd53733e5a3.js",
             "style": "./style"
         },
         "disabledExtensions": [
             "jupyterlab-myst:plugin",
             "jupyterlab-myst:legacyPlugin",
             "jupyterlab-myst:executor"
         ],
@@ -188,9 +188,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.5"
+    "version": "0.2.7"
 }
```

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/11.bbf21e9c517bec162b9c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/136.43b409c7c7e6885bc7ee.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/150.9b2f6283ffc934651e1c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/185.a8ca3522cb5c31423453.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/3.b7aa6beb2ddb69469e1e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/316.f7e4dd762f98107da4a5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/384.6c76694e25edf7010d50.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/487.dee02fd512e9bb15dee6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/543.40a7a1799fcad108039e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/573.79885c9e9fcb552239cd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/596.ef22233afe464ab9134a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/645.406375856388e9d7e4e9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/651.7673e27b3217024cb32d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/700.30097f2c1808e10c985f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/724.265325864c2c7d67e29e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/923.b51eb181f4c017b19c97.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/980.57fcdfda225b581383c0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/remoteEntry.ee954710581352bf9b27.js` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/remoteEntry.110f607f4dd53733e5a3.js`

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
-                return "default" === r && (f("jupyterlab-quarto", "0.2.5", (() => Promise.all([P.e(185), P.e(573), P.e(150), P.e(923)]).then((() => () => P(5923))))), f("markdown-it-attrs", "4.1.6", (() => P.e(543).then((() => () => P(9543))))), f("markdown-it-deflist", "2.1.0", (() => P.e(645).then((() => () => P(645))))), f("markdown-it-footnote", "3.0.3", (() => P.e(384).then((() => () => P(2384))))), f("markdown-it-sub", "1.0.0", (() => P.e(700).then((() => () => P(700))))), f("markdown-it-sup", "1.0.0", (() => P.e(3).then((() => () => P(7003))))), f("markdown-it-task-lists", "1.4.1", (() => P.e(651).then((() => () => P(4651))))), f("markdown-it", "12.3.2", (() => Promise.all([P.e(980), P.e(185)]).then((() => () => P(9980))))), f("mermaid", "9.4.3", (() => P.e(136).then((() => () => P(4136))))), f("wcwidth", "1.0.1", (() => P.e(11).then((() => () => P(1011)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
+                return "default" === r && (f("jupyterlab-quarto", "0.2.7", (() => Promise.all([P.e(185), P.e(573), P.e(150), P.e(923)]).then((() => () => P(5923))))), f("markdown-it-attrs", "4.1.6", (() => P.e(543).then((() => () => P(9543))))), f("markdown-it-deflist", "2.1.0", (() => P.e(645).then((() => () => P(645))))), f("markdown-it-footnote", "3.0.3", (() => P.e(384).then((() => () => P(2384))))), f("markdown-it-sub", "1.0.0", (() => P.e(700).then((() => () => P(700))))), f("markdown-it-sup", "1.0.0", (() => P.e(3).then((() => () => P(7003))))), f("markdown-it-task-lists", "1.4.1", (() => P.e(651).then((() => () => P(4651))))), f("markdown-it", "12.3.2", (() => Promise.all([P.e(980), P.e(185)]).then((() => () => P(9980))))), f("mermaid", "9.4.3", (() => P.e(136).then((() => () => P(4136))))), f("wcwidth", "1.0.1", (() => P.e(11).then((() => () => P(1011)))))), e[r] = i.length ? Promise.all(i).then((() => e[r] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var t = P.g.document;
         if (!e && t && (t.currentScript && (e = t.currentScript.src), !e)) {
```

### Comparing `jupyterlab_quarto-0.2.5/jupyterlab-quarto/labextension/static/third-party-licenses.json` & `jupyterlab_quarto-0.2.7/jupyterlab-quarto/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/index.ts` & `jupyterlab_quarto-0.2.7/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/manager.ts` & `jupyterlab_quarto-0.2.7/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/types.ts` & `jupyterlab_quarto-0.2.7/src/types.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/widgets.ts` & `jupyterlab_quarto-0.2.7/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/ast/ast.ts` & `jupyterlab_quarto-0.2.7/src/ast/ast.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/hooks/codemirror.ts` & `jupyterlab_quarto-0.2.7/src/hooks/codemirror.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/callouts.ts` & `jupyterlab_quarto-0.2.7/src/plugins/callouts.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/cites.ts` & `jupyterlab_quarto-0.2.7/src/plugins/cites.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/decorator.ts` & `jupyterlab_quarto-0.2.7/src/plugins/decorator.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/divs.ts` & `jupyterlab_quarto-0.2.7/src/plugins/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/figure-divs.ts` & `jupyterlab_quarto-0.2.7/src/plugins/figure-divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/figures.ts` & `jupyterlab_quarto-0.2.7/src/plugins/figures.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/index.ts` & `jupyterlab_quarto-0.2.7/src/plugins/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/math.ts` & `jupyterlab_quarto-0.2.7/src/plugins/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/shortcodes.ts` & `jupyterlab_quarto-0.2.7/src/plugins/shortcodes.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/spans.ts` & `jupyterlab_quarto-0.2.7/src/plugins/spans.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/table-captions.ts` & `jupyterlab_quarto-0.2.7/src/plugins/table-captions.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/yaml.ts` & `jupyterlab_quarto-0.2.7/src/plugins/yaml.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/index.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/gridtables/GetCells.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetCells.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/gridtables/GetColumnWidths.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/EmitTable.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/EmitTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetCharCodeAtStartOfLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/GetLine.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/GetLine.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/ParseTable.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/common/markdown-it/ParseTableResult.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/interfaces/markdown-it/IState.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/IState.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/interfaces/markdown-it/TRuleFunction.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/gridtables/rules/gridtable.ts` & `jupyterlab_quarto-0.2.7/src/plugins/gridtables/rules/gridtable.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/mermaid/index.ts` & `jupyterlab_quarto-0.2.7/src/plugins/mermaid/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/utils/html.ts` & `jupyterlab_quarto-0.2.7/src/plugins/utils/html.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/plugins/utils/markdownit.ts` & `jupyterlab_quarto-0.2.7/src/plugins/utils/markdownit.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/providers/divs.ts` & `jupyterlab_quarto-0.2.7/src/providers/divs.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/providers/math.ts` & `jupyterlab_quarto-0.2.7/src/providers/math.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/src/providers/provider.ts` & `jupyterlab_quarto-0.2.7/src/providers/provider.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/style/base.css` & `jupyterlab_quarto-0.2.7/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/ui-tests/README.md` & `jupyterlab_quarto-0.2.7/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/ui-tests/tests/jupyterlab-quarto.spec.ts` & `jupyterlab_quarto-0.2.7/ui-tests/tests/jupyterlab-quarto.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/.gitignore` & `jupyterlab_quarto-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/LICENSE` & `jupyterlab_quarto-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/README.md` & `jupyterlab_quarto-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/pyproject.toml` & `jupyterlab_quarto-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_quarto-0.2.5/PKG-INFO` & `jupyterlab_quarto-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-quarto
-Version: 0.2.5
+Version: 0.2.7
 Summary: Jupyter extension to enable authoring of Quarto documents within Jupyterlab Notebooks.
 Project-URL: Homepage, https://github.com/quarto-dev/jupyterlab-quarto
 Project-URL: Bug Tracker, https://github.com/quarto-dev/jupyterlab-quarto/issues
 Project-URL: Repository, https://github.com/quarto-dev/jupyterlab-quarto.git
 Author-email: Charles Teague <charles@posit.co>
 License: BSD 3-Clause License
```

