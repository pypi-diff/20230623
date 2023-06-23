# Comparing `tmp/jupyterlab_nbqueue-0.1.6.tar.gz` & `tmp/jupyterlab_nbqueue-0.1.7.tar.gz`

## Comparing `jupyterlab_nbqueue-0.1.6.tar` & `jupyterlab_nbqueue-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/.bxplorer.db
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/.jupyterlab-nbqueue.db
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/RELEASE.md
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/RunningCode.ipynb
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/install.json
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/setup.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/test04.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/tsconfig.json
--rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/yarn.lock
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyter-config/nb-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyter-config/server-config/jupyterlab_nbqueue.json
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/_version.py
--rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/cmd_launcher.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/db_handler.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/handlers.py
--rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/build_log.json
--rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/package.json
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
--rw-r--r--   0        0        0    63566 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js
--rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map
--rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js
--rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/style.js
--rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
--rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
--rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
--rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
--rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
--rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/handler.ts
--rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/index.ts
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/svg.d.ts
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/components/CustomProps.tsx
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/components/RunComponent.tsx
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/components/RunsContext.tsx
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/components/RunsPanelComponent.tsx
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/components/runs.ts
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/style/IconsStyle.ts
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/src/widgets/RunsPanelWidget.tsx
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/base.css
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/index.js
--rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/nbqueue_logo_v1.svg
--rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/nbqueue_logo_v2.svg
--rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/css/all.css
--rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/css/fontawesome.css
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/css/solid.css
--rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/js/fontawesome.js
--rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/js/pro.js
--rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/js/solid.js
--rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/style/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/LICENSE
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/README.md
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/.bxplorer.db
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/.jupyterlab-nbqueue.db
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/RELEASE.md
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/RunningCode.ipynb
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/install.json
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/setup.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/test04.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/tsconfig.json
+-rw-r--r--   0        0        0   209091 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/yarn.lock
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyter-config/nb-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyter-config/server-config/jupyterlab_nbqueue.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/_version.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/cmd_launcher.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/db_handler.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/handlers.py
+-rw-r--r--   0        0        0    22112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/build_log.json
+-rw-r--r--   0        0        0     5737 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/package.json
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/77df7d949de7b5ae43b0.woff2
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/8be134a2ed7f85fceac5.ttf
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf
+-rw-r--r--   0        0        0    63566 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js
+-rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map
+-rw-r--r--   0        0        0    30547 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js
+-rw-r--r--   0        0        0    29341 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/style.js
+-rw-r--r--   0        0        0   439063 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js
+-rw-r--r--   0        0        0   529754 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map
+-rw-r--r--   0        0        0  1074536 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js
+-rw-r--r--   0        0        0  1311425 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map
+-rw-r--r--   0        0        0   426094 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js
+-rw-r--r--   0        0        0   332375 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/handler.ts
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/index.ts
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/svg.d.ts
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/components/CustomProps.tsx
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/components/RunComponent.tsx
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/components/RunsContext.tsx
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/components/RunsPanelComponent.tsx
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/components/runs.ts
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/style/IconsStyle.ts
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/src/widgets/RunsPanelWidget.tsx
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/base.css
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/index.js
+-rw-r--r--   0        0        0    16753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/nbqueue_logo_v1.svg
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/nbqueue_logo_v2.svg
+-rw-r--r--   0        0        0   966058 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/css/all.css
+-rw-r--r--   0        0        0   163322 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/css/fontawesome.css
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/css/solid.css
+-rw-r--r--   0        0        0   105753 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/js/fontawesome.js
+-rw-r--r--   0        0        0   125539 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/js/pro.js
+-rw-r--r--   0        0        0  1794940 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/js/solid.js
+-rw-r--r--   0        0        0   648356 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   279576 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0   270360 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/style/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/README.md
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6200 2020-02-02 00:00:00.000000 jupyterlab_nbqueue-0.1.7/PKG-INFO
```

### Comparing `jupyterlab_nbqueue-0.1.6/.bxplorer.db` & `jupyterlab_nbqueue-0.1.7/.bxplorer.db`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/.jupyterlab-nbqueue.db` & `jupyterlab_nbqueue-0.1.7/.jupyterlab-nbqueue.db`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/RELEASE.md` & `jupyterlab_nbqueue-0.1.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/RunningCode.ipynb` & `jupyterlab_nbqueue-0.1.7/RunningCode.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/package.json` & `jupyterlab_nbqueue-0.1.7/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.7'"}*

```diff
@@ -183,9 +183,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.6"
+    "version": "0.1.7"
 }
```

### Comparing `jupyterlab_nbqueue-0.1.6/test04.ipynb` & `jupyterlab_nbqueue-0.1.7/test04.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/tsconfig.json` & `jupyterlab_nbqueue-0.1.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/yarn.lock` & `jupyterlab_nbqueue-0.1.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/__init__.py` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/cmd_launcher.py` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/cmd_launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,19 @@
                 session.commit()
                               
                 out, error = process.communicate()
                 logger.info('************ BEGIN process.communicate ************')
                 logger.info(out)
                 logger.info(error)
                 logger.info('************ END process.communicate ************')
-                # if error.strip() != '':
-                #     session.query(Runs).filter_by(pid=process.pid).update({'status': 'Error', 'message': 'ERROR'})
+                if error.strip() != '':
+                    session.query(Runs).filter_by(pid=process.pid).update({'status': 'Error', 'message': error.strip().encode('utf-8')})
 
-                # if out.strip() != '':
-                #     session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
-                session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
+                if out.strip() != '':
+                    session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
+                # session.query(Runs).filter_by(pid=process.pid).update({'status': 'Finished'})
 
                 session.commit()
             else:
                 logger.info("It has not been possible to execute the command. It must be related to the OS")
                 print("It has not been possible to execute the command. It must be related to the OS")
```

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/db_handler.py` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/db_handler.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/handlers.py` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/build_log.json` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/package.json` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/4dd3561bac1f21c70270e2f4d93e30b9eaa7538b5fb12b6f6d5d9a74033e5750.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/db04c49278de66fe78d2bfebf2ea48cea5ea5278071b87bb757d1fad6ad045f4.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/lib_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8_8-ebac61.91b22bf331b9da31ee2c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/remoteEntry.91acc9f63b6c5a36112b.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/style_index_js-data_image_svg_xml_3csvg_xmlns_27http_www_w3_org_2000_svg_27_viewBox_27-4_-4_8-b1efa1.3970d5aff54335b54c0d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_css-loader_dist_cjs_js_node_modules_bootstrap_dist_css_bootstrap_min_css-07a54b.103775b5d2edfd3cd852.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map` & `jupyterlab_nbqueue-0.1.7/jupyterlab_nbqueue/labextension/static/vendors-node_modules_react-bootstrap_esm_Button_js-node_modules_react-bootstrap_esm_ButtonGro-f50093.766984a3c69834ca0c09.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/src/handler.ts` & `jupyterlab_nbqueue-0.1.7/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/src/index.ts` & `jupyterlab_nbqueue-0.1.7/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/src/components/RunComponent.tsx` & `jupyterlab_nbqueue-0.1.7/src/components/RunComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/src/components/RunsContext.tsx` & `jupyterlab_nbqueue-0.1.7/src/components/RunsContext.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/src/components/RunsPanelComponent.tsx` & `jupyterlab_nbqueue-0.1.7/src/components/RunsPanelComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/src/widgets/RunsPanelWidget.tsx` & `jupyterlab_nbqueue-0.1.7/src/widgets/RunsPanelWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/nbqueue_logo_v1.svg` & `jupyterlab_nbqueue-0.1.7/style/nbqueue_logo_v1.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/nbqueue_logo_v2.svg` & `jupyterlab_nbqueue-0.1.7/style/nbqueue_logo_v2.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/css/all.css` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/css/all.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/css/fontawesome.css` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/css/solid.css` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/js/fontawesome.js` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/js/pro.js` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/js/pro.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/js/solid.js` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/js/solid.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/webfonts/fa-solid-900.ttf` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/webfonts/fa-solid-900.woff` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/style/fontawesome/webfonts/fa-solid-900.woff2` & `jupyterlab_nbqueue-0.1.7/style/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/.gitignore` & `jupyterlab_nbqueue-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/LICENSE` & `jupyterlab_nbqueue-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/README.md` & `jupyterlab_nbqueue-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/pyproject.toml` & `jupyterlab_nbqueue-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nbqueue-0.1.6/PKG-INFO` & `jupyterlab_nbqueue-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nbqueue
-Version: 0.1.6
+Version: 0.1.7
 Summary: A JupyterLab extension for queuing notebooks executions.
 Project-URL: Homepage, https://github.com/Navteca/jupyterlab-nbqueue.git
 Project-URL: Bug Tracker, https://github.com/Navteca/jupyterlab-nbqueue.git/issues
 Project-URL: Repository, https://github.com/Navteca/jupyterlab-nbqueue.git.git
 Author-email: Navteca LLC <info@navteca.com>
 License: BSD 3-Clause License
```

