# Comparing `tmp/documenteer-0.8.0b2.tar.gz` & `tmp/documenteer-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-0.8.0b2.tar", last modified: Wed Mar  1 15:51:31 2023, max compression
+gzip compressed data, was "documenteer-1.0.0a1.tar", last modified: Wed Jun  7 19:12:56 2023, max compression
```

## Comparing `documenteer-0.8.0b2.tar` & `documenteer-1.0.0a1.tar`

### file list

```diff
@@ -1,255 +1,258 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/demo/rst-technote/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.170154 documenteer-0.8.0b2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.170154 documenteer-0.8.0b2/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.170154 documenteer-0.8.0b2/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxconfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/html-templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/theme-assets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/theme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.174154 documenteer-0.8.0b2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.174154 documenteer-0.8.0b2/docs/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/stack-docs-cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/docs/technotes/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/technotes/refresh-lsst-bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-03-01 15:51:14.000000 documenteer-0.8.0b2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/assets/rubin-technote/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/src/assets/rubin-technote/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/_properties.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/_index.scss
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/_version-info.scss
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/rubin-technote.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/bin/buildstackdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/bin/refreshlsstbib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/technote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/technotebeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/sphinxconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.190154 documenteer-0.8.0b2/src/documenteer/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.190154 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.190154 documenteer-0.8.0b2/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/pydata/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/technote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/technote/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/components/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.198154 documenteer-0.8.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.198154 documenteer-0.8.0b2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/roots/test-autocppapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_ext_autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_refreshlsstbib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxconfig_stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_lsstdocushare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_lssttasks_taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29338 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.718858 documenteer-1.0.0a1/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29338 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.730858 documenteer-1.0.0a1/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/pipelines/stack-docs-cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/openapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/docs/technotes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/docs/technotes/refresh-lsst-bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-06-07 19:12:44.000000 documenteer-1.0.0a1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.734858 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/assets/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-07 19:12:46.000000 documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/buildstackdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/bin/refreshlsstbib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17519 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/technote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/conf/technotebeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/ext/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxconfig/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.742858 documenteer-1.0.0a1/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.746858 documenteer-1.0.0a1/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/components/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.750858 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.738858 documenteer-1.0.0a1/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 19:12:56.000000 documenteer-1.0.0a1/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.758858 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.722858 documenteer-1.0.0a1/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.726858 documenteer-1.0.0a1/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:12:56.762858 documenteer-1.0.0a1/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/roots/test-autocppapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_ext_autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_refreshlsstbib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxconfig_stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_lsstdocushare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_lssttasks_taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_sphinxext_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tests/test_technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-07 19:12:35.000000 documenteer-1.0.0a1/webpack.config.js
```

### Comparing `documenteer-0.8.0b2/.github/workflows/ci-cron.yaml` & `documenteer-1.0.0a1/.github/workflows/ci-cron.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/.github/workflows/ci.yaml` & `documenteer-1.0.0a1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/.gitignore` & `documenteer-1.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/.pre-commit-config.yaml` & `documenteer-1.0.0a1/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies:
           - toml
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
@@ -34,11 +34,11 @@
 
   - repo: https://github.com/pycqa/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: 'v3.0.0-alpha.4'
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
         types_or: [css, scss, javascript]
```

### Comparing `documenteer-0.8.0b2/.vscode/tasks.json` & `documenteer-1.0.0a1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/CHANGELOG.md` & `documenteer-1.0.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 ## Unreleased
 
 - Add a new `documenteer.conf.technotebeta` configuration for [technote](https://technote.lsst.io)-based technotes.
   These technotes are now themed with Rubin's modern branding.
 - Drop support for Python 3.7.
 - Drop support for Sphinx versions earlier than 5.
 - Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
+- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds.
+- Add a new `sphinx.exclude` field to `documenteer.toml` to list files for exclusion from a documentation project.
+  More files and directories like `.venv` and `requirements.txt` are now excluded, as well.
+- New support for embedding OpenAPI documentation in a Redoc-generated subsite. The `documenteer.ext.openapi` extension can call a user-specified function to generate and install the OpenAPI specification the Sphinx source. For user guide projects, the `[project.openapi]` table in `documenteer.toml` can be used to configure both the `documenteer.ext.openapi` and `sphinxcontrib-redoc` extensions. [sphinxcontrib-redoc](https://sphinxcontrib-redoc.readthedocs.io/en/stable/) is installed and configured by default for all Rubin user guide projects (projects that use `documenteer.conf.guide`).
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
```

### Comparing `documenteer-0.8.0b2/LICENSE` & `documenteer-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/PKG-INFO` & `documenteer-1.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 0.8.0b2
+Version: 1.0.0a1
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-0.8.0b2/README.md` & `documenteer-1.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/demo/rst-technote/index.rst` & `documenteer-1.0.0a1/demo/rst-technote/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/Makefile` & `documenteer-1.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/_rst_epilog.rst` & `documenteer-1.0.0a1/docs/_rst_epilog.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. Links and substitutions available from every rst page
 
 .. External links
 
 .. _Doxygen: http://www.doxygen.nl
 .. _Doxylink: https://sphinxcontrib-doxylink.readthedocs.io/en/stable/
+.. _FastAPI: https://fastapi.tiangolo.com
 .. _Intersphinx: https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html
-.. _LSST Science Pipelines:
 .. _SCons: https://scons.org
 .. _Sphinx extensions: https://www.sphinx-doc.org/en/master/develop.html
 .. _Sphinx: https://www.sphinx-doc.org/en/master/
 .. _Mermaid: https://mermaid-js.github.io/mermaid/#/
 .. _sphinxcontrib-mermaid: https://github.com/mgaitan/sphinxcontrib-mermaid
 .. _Diagrams: https://diagrams.mingrammer.com/
 .. _sphinx-diagrams: https://github.com/j-martin/sphinx-diagrams
@@ -27,14 +27,15 @@
 .. _TOML: https://toml.io/en/
 .. _`SQR-006`: https://sqr-006.lsst.io
 .. _`lsstDoxygen`: https://github.com/lsst/lsstDoxygen
 .. _`package-docs`: https://documenteer.lsst.io/pipelines/package-docs-cli.html
 .. _`pex_config`: https://github.com/lsst/pex_config
 .. _`pipe_base`: https://github.com/lsst/pipe_base
 .. _`pipe_supertask`: https://github.com/lsst/pipe_supertask
+.. _LSST Science Pipelines:
 .. _`pipelines.lsst.io`: https://pipelines.lsst.io
 .. _`pipelines_lsst_io`: https://github.com/lsst/pipelines_lsst_io
 .. _`sconsUtils`: https://github.com/lsst/sconsUtils
 .. _`sqre/infrastructure/documenteer`: https://ci.lsst.codes/blue/organizations/jenkins/sqre%2Finfrastructure%2Fdocumenteer/activity
 .. _astro-metadata-translator.lsst.io: https://astro-metadata-translator.lsst.io
 .. _automodapi: http://sphinx-automodapi.readthedocs.io/en/latest/automodapi.html
 .. _black: https://black.readthedocs.io/en/stable/
@@ -43,18 +44,20 @@
 .. _conda: https://conda.io/en/latest/index.html
 .. _isort: https://pycqa.github.io/isort/
 .. _numpydoc: https://numpydoc.readthedocs.io/en/latest/index.html
 .. _pre-commit: https://pre-commit.com
 .. _pytest: https://pytest.org
 .. _toctree: http://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#directive-toctree
 .. _linkcheck: https://www.sphinx-doc.org/en/master/usage/configuration.html?#options-for-the-linkcheck-builder
+.. _Redoc: https://redocly.com/redoc/
 .. _rst_epilog: https://www.sphinx-doc.org/en/master/usage/configuration.html?highlight=rst_epilog#confval-rst_epilog
 .. _napoleon: https://www.sphinx-doc.org/en/master/usage/extensions/napoleon.html
 .. _autodoc: https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html
 .. _sphinx_autodoc_typehints: https://github.com/tox-dev/sphinx-autodoc-typehints
+.. _sphinxcontrib-redoc: https://sphinxcontrib-redoc.readthedocs.io/en/stable/
 .. _tox: https://tox.wiki/en/latest/
 .. _Technote: https://technote.lsst.io/
 
 .. Internal links
 
 .. |documenteer.toml| replace:: :doc:`documenteer.toml </guides/toml-reference>`
 .. |documenteer.conf.guide| replace:: :doc:`documenteer.conf.guide </guides/configuration-preset>`
```

### Comparing `documenteer-0.8.0b2/docs/changelog.md` & `documenteer-1.0.0a1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 ## Unreleased
 
 - Add a new `documenteer.conf.technotebeta` configuration for [technote](https://technote.lsst.io)-based technotes.
   These technotes are now themed with Rubin's modern branding.
 - Drop support for Python 3.7.
 - Drop support for Sphinx versions earlier than 5.
 - Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
+- Use [sphinxcontrib-jquery](https://github.com/sphinx-contrib/jquery/) to ensure jQuery is available for user guide and Pipelines documentation builds.
+- Add a new `sphinx.exclude` field to `documenteer.toml` to list files for exclusion from a documentation project.
+  More files and directories like `.venv` and `requirements.txt` are now excluded, as well.
+- New support for embedding OpenAPI documentation in a Redoc-generated subsite. The `documenteer.ext.openapi` extension can call a user-specified function to generate and install the OpenAPI specification the Sphinx source. For user guide projects, the `[project.openapi]` table in `documenteer.toml` can be used to configure both the `documenteer.ext.openapi` and `sphinxcontrib-redoc` extensions. [sphinxcontrib-redoc](https://sphinxcontrib-redoc.readthedocs.io/en/stable/) is installed and configured by default for all Rubin user guide projects (projects that use `documenteer.conf.guide`).
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
```

### Comparing `documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxext.rst` & `documenteer-1.0.0a1/docs/dev/api/documenteer.sphinxext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-1.0.0a1/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/dev/development.rst` & `documenteer-1.0.0a1/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/dev/html-templates.rst` & `documenteer-1.0.0a1/docs/dev/html-templates.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/dev/release.rst` & `documenteer-1.0.0a1/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/dev/theme-assets.rst` & `documenteer-1.0.0a1/docs/dev/theme-assets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/documenteer.toml` & `documenteer-1.0.0a1/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/badges.rst` & `documenteer-1.0.0a1/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/configuration.rst` & `documenteer-1.0.0a1/docs/guides/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/diagrams.rst` & `documenteer-1.0.0a1/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/extend-conf-py.rst` & `documenteer-1.0.0a1/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/index.rst` & `documenteer-1.0.0a1/docs/guides/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: Advanced configuration
    :name: toc-guides-advanced-config
 
    pyproject-configuration
+   openapi
    rst-epilog
    extend-conf-py
 
 .. toctree::
    :maxdepth: 2
    :caption: Design features
    :name: toc-guides-design
```

### Comparing `documenteer-0.8.0b2/docs/guides/organization.rst` & `documenteer-1.0.0a1/docs/guides/organization.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/overview.rst` & `documenteer-1.0.0a1/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/pyproject-configuration.rst` & `documenteer-1.0.0a1/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/rst-epilog.rst` & `documenteer-1.0.0a1/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/tabsets.rst` & `documenteer-1.0.0a1/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/guides/toml-reference.rst` & `documenteer-1.0.0a1/docs/guides/toml-reference.rst`

 * *Files 16% similar despite different names*

```diff
@@ -83,14 +83,101 @@
 version
 -------
 
 |optional| |py-auto|
 
 The project's version, which is set to the standard Sphinx ``version`` and ``release`` configuration variables.
 
+.. _guide-project-openapi:
+
+[project.openapi]
+=================
+
+|optional|
+
+Web applications that use OpenAPI can include a ``[project.openapi]`` table in :file:`documenteer.toml` to embed a Redoc_ subsite of the API documentation (see :doc:`openapi`).
+
+.. _guide-project-openapi-doc-path:
+
+doc\_path
+---------
+
+|optional|
+
+The docname (without extension) of the page in the Sphinx documentation tree where the Redoc HTML page is built.
+Default is ``api``.
+
+.. _guide-project-openapi-openapi-path:
+
+openapi\_path
+-------------
+
+|optional|
+
+The path to the OpenAPI specification file, relative to the Sphinx configuration file, :file:`conf.py`.
+If ``[project.openapi.generator]`` is set, this is the path where the OpenAPI specification file is generated.
+
+.. _guide-project-openapi-generator:
+
+[project.openapi.generator]
+===========================
+
+|optional|
+
+If this table is provided, the OpenAPI specification file is generated from a user-specified Python function.
+This is useful for FastAPI and similar applications where the OpenAPI specification is generated from the application code.
+
+.. _guide-project-openapi-generator-function:
+
+function
+--------
+
+|required|
+
+The Python function that generates the OpenAPI specification file.
+This function must return the OpenAPI specification as a JSON-serialized string.
+
+Specify the function as ``<module>:<function>``.
+For example, if the function called ``create_openapi`` is in the :file:`main.py` module of the :file:`example` package, the value would be ``"example.main:create_openapi"``.
+
+.. code-block:: toml
+
+   [project.openapi.generator]
+   function = "example.main:create_openapi"
+
+.. _guide-project-openapi-generator-positional-args:
+
+positional\_args
+----------------
+
+|optional|
+
+Positional arguments to pass to the function, if required.
+
+.. code-block:: toml
+
+   [project.openapi.generator]
+   function = "example.main:create_openapi"
+   positional_args = ["arg1", "arg2"]
+
+.. _guide-project-openapi-generator-keyword-args:
+
+keyword\_args
+-------------
+
+|optional|
+
+Keyword arguments to pass to the function, if required.
+
+.. code-block:: toml
+
+   [project.openapi.generator]
+   function = "example.main:create_openapi"
+   keyword_args = {kwarg1 = "value1", kwarg2 = "value2"}
+
 [project.python]
 ================
 
 |optional|
 
 Projects that use a :file:`pyproject.toml` to set their build metadata can include a ``[project.python]`` table in :file:`documenteer.toml`.
 With this, many metadata values are automatically detected — look for |py-auto| badges above.
@@ -161,14 +248,23 @@
    ]
 
 .. note::
 
    This configuration is for the **primary** sidebar, on the left side, containing side or section-level navigation links.
    To remove the page-level contents sidebar, on the right side, add ``:html_theme.sidebar_secondary.remove:`` to the *page's* file metadata.
 
+exclude
+-------
+
+|optional|
+
+A list of file paths, relative to :file:`conf.py`, to exclude from the Sphinx build.
+This configuration is often used to prevent file unrelated to the documentation from being accidentally included in the site build.
+|documenteer.conf.guide| includes common files and directories, so you may not need to modify this configuration in standard situations.
+
 extensions
 ----------
 
 |optional|
 
 A list of Sphinx extensions to append to the extensions included in the Documenteer configuration preset (see |documenteer.conf.guide|).
 Duplicate extensions are ignored.
```

### Comparing `documenteer-0.8.0b2/docs/index.rst` & `documenteer-1.0.0a1/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ###########
 Documenteer
 ###########
 
 **Sphinx extensions, configurations, and tooling for Rubin Observatory documentation projects.**
 
 Documenteer is developed on GitHub at https://github.com/lsst-sqre/documenteer.
-Find other version of the documentation at https://documenteer.lsst.io/v
+Find other versions of the documentation at https://documenteer.lsst.io/v
 
 .. _pip-install:
 .. _installation:
 
 Installation
 ============
```

### Comparing `documenteer-0.8.0b2/docs/pipelines/build-overview.rst` & `documenteer-1.0.0a1/docs/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/pipelines/configuration.rst` & `documenteer-1.0.0a1/docs/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/pipelines/cpp-api-linking.rst` & `documenteer-1.0.0a1/docs/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/pipelines/index.rst` & `documenteer-1.0.0a1/docs/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/pipelines/install.rst` & `documenteer-1.0.0a1/docs/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/pipelines/package-docs-cli.rst` & `documenteer-1.0.0a1/docs/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/pipelines/stack-docs-cli.rst` & `documenteer-1.0.0a1/docs/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/autocppapi.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/autodocreset.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/jira-reference.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/jira-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/lssttasks.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/package-toctree.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-1.0.0a1/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/technotes/configuration.rst` & `documenteer-1.0.0a1/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/technotes/index.rst` & `documenteer-1.0.0a1/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/docs/technotes/refresh-lsst-bib.rst` & `documenteer-1.0.0a1/docs/technotes/refresh-lsst-bib.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/licenses/astropy-helpers.txt` & `documenteer-1.0.0a1/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/licenses/sphinx-issue.txt` & `documenteer-1.0.0a1/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/licenses/sphinx.txt` & `documenteer-1.0.0a1/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/package-lock.json` & `documenteer-1.0.0a1/package-lock.json`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/package.json` & `documenteer-1.0.0a1/package.json`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/pyproject.toml` & `documenteer-1.0.0a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     "sphinx-automodapi",
     "sphinx-copybutton",
     "sphinx-prompt",
     "myst-parser",
     "markdown-it-py[linkify]",
     "sphinxcontrib-mermaid",
     "sphinxext-opengraph",
+    "sphinxcontrib-redoc",
+    "sphinxcontrib-jquery",
 ]
 technote = [
     # Theme and extensions for technotes
     "lsst-dd-rtd-theme>=0.2.3,<0.3.0",
     "technote>=0.2.0",
     "sphinx-prompt",
 ]
@@ -82,14 +84,15 @@
     "numpydoc",
     "sphinx-automodapi",
     "sphinx-jinja",
     "sphinxcontrib-autoprogram",
     "sphinx-prompt",
     "sphinxcontrib-doxylink",
     "sphinx-click",
+    "sphinxcontrib-jquery",
 ]
 
 [project.urls]
 Homepage = "https://documenteer.lsst.io"
 Source = "https://github.com/lsst-sqre/documenteer"
 
 [project.scripts]
@@ -163,7 +166,8 @@
 disallow_incomplete_defs = true
 ignore_missing_imports = true
 show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_ignores = true
+plugins = ["pydantic.mypy"]
```

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/favicon.ico` & `documenteer-1.0.0a1/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-1.0.0a1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js` & `documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js.map` & `documenteer-1.0.0a1/src/documenteer/assets/scripts/rubin-technote.js.map`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css` & `documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css.map` & `documenteer-1.0.0a1/src/documenteer/assets/styles/rubin-technote.css.map`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/bin/buildstackdocs.py` & `documenteer-1.0.0a1/src/documenteer/bin/buildstackdocs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/bin/refreshlsstbib.py` & `documenteer-1.0.0a1/src/documenteer/bin/refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/_toml.py` & `documenteer-1.0.0a1/src/documenteer/conf/_toml.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,15 +41,79 @@
     ValidationError,
     validator,
 )
 from sphinx.errors import ConfigError
 
 from ._utils import GitRepository
 
-__all__ = ["ProjectModel", "ConfigRoot", "DocumenteerConfig"]
+__all__ = [
+    "ConfigRoot",
+    "DocumenteerConfig",
+    "ProjectModel",
+    "PythonPackageModel",
+    "OpenApiDocsModel",
+    "OpenApiGeneratorModel",
+    "SphinxModel",
+    "IntersphinxModel",
+    "LinkCheckModel",
+    "ThemeModel",
+]
+
+
+class OpenApiGeneratorModel(BaseModel):
+    """Specification for the OpenAPI generator function used by the
+    ``documenteer.ext.openapi`` Sphinx extension.
+    """
+
+    function: str = Field(
+        description=(
+            "The Python function that generates the OpenAPI spec file. "
+            "It must have the form ``module:func``. The function must return "
+            "a JSON-serialized string."
+        )
+    )
+
+    positional_args: List[Any] = Field(
+        default_factory=list,
+        description=(
+            "Positional arguments to pass to the generator function."
+        ),
+    )
+
+    keyword_args: Dict[str, Any] = Field(
+        default_factory=dict,
+        description=("Keyword arguments to pass to the generator function."),
+    )
+
+
+class OpenApiDocsModel(BaseModel):
+    """Model for OpenAPI documentation configurations in documenteer.toml."""
+
+    generator: Optional[OpenApiGeneratorModel] = Field(
+        None,
+        description=(
+            "The function that generates the OpenAPI spec file from the"
+            "application source code. If not specified, the OpenAPI spec file "
+            "assumed to be generated by an external process and provided at "
+            "the path specified by ``openapi_path``."
+        ),
+    )
+
+    openapi_path: str = Field(
+        "_static/openapi.json",
+        description=(
+            "This is the path, relative to the Sphinx conf.py file, where the "
+            "OpenAPI spec file is written. Default is "
+            "``_static/openapi.json``."
+        ),
+    )
+
+    doc_path: str = Field(
+        "api",
+    )
 
 
 class PythonPackageModel(BaseModel):
     """Model for a Python package (i.e. built with pyproject.toml-compatible
     build system.
     """
 
@@ -110,15 +174,17 @@
     github_default_branch: str = Field(
         "main",
         description="The project's default development branch on GitHub.",
     )
 
     version: Optional[str] = Field(description="Version string.")
 
-    python: Optional[PythonPackageModel]
+    python: Optional[PythonPackageModel] = Field(None)
+
+    openapi: Optional[OpenApiDocsModel] = Field(None)
 
 
 class IntersphinxModel(BaseModel):
     """Model for Intersphinx configurations in documenteer.toml."""
 
     projects: Dict[str, HttpUrl] = Field(
         description="Mapping of projects and their URLs.", default_factory=dict
@@ -198,14 +264,22 @@
         None,
         description=(
             "Directory path where the Python API reference documentation "
             "is created."
         ),
     )
 
+    exclude: List[str] = Field(
+        description=(
+            "List of paths to exclude from being considered as Sphinx content "
+            "sources."
+        ),
+        default_factory=list,
+    )
+
     theme: ThemeModel = Field(default_factory=lambda: ThemeModel())
 
     intersphinx: Optional[IntersphinxModel]
 
     linkcheck: Optional[LinkCheckModel]
 
 
@@ -402,14 +476,21 @@
     @property
     def nitpicky(self) -> bool:
         if self.conf.sphinx:
             return self.conf.sphinx.nitpicky
         else:
             return False
 
+    def extend_exclude_patterns(self, exclude_patterns: List[str]) -> None:
+        """Extend Sphinx ``exclude_patterns`` with the "exclude" configuration
+        from the sphinx TOML table.
+        """
+        if self.conf.sphinx and self.conf.sphinx.exclude:
+            exclude_patterns.extend(self.conf.sphinx.exclude)
+
     def disable_primary_sidebars(
         self, html_sidebars: MutableMapping[str, List[str]]
     ) -> None:
         if self.conf.sphinx and self.conf.sphinx.disable_primary_sidebars:
             pages = self.conf.sphinx.disable_primary_sidebars
         else:
             pages = ["index"]  # default
```

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/_utils.py` & `documenteer-1.0.0a1/src/documenteer/conf/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/guide.py` & `documenteer-1.0.0a1/src/documenteer/conf/guide.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 To use this configuration in a Sphinx technote project, write a conf.py
 containing::
 
     from documenteer.conf.guide import *
 """
 
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from documenteer.conf import (
     DocumenteerConfig,
     get_asset_path,
     get_template_dir,
 )
 
@@ -30,14 +30,16 @@
 #     API reference configuration
 # #MYST
 #     MyST markdown configurations
 # #MERMIAID
 #     Mermaid diagram support
 # #OPENGRAPH
 #     OpenGraph metadata support
+# #OPENAPI
+#     OpenAPI/redoc support
 
 
 # Ordered as they are declared in this module
 __all__ = [
     # EXT
     "extensions",
     # SPHINX
@@ -98,40 +100,48 @@
     # MERMAID
     "mermaid_output_format",
     "mermaid_version",
     # OPENGRAPH
     "ogp_site_url",
     "ogp_site_name",
     "ogp_use_first_image",
+    # OPENAPI
+    "documenteer_openapi_generator",
+    "documenteer_openapi_path",
+    "redoc",
+    "redoc_uri",
 ]
 
 _conf = DocumenteerConfig.find_and_load()
 
 
 # ============================================================================
 # #EXT Sphinx extensions
 # ============================================================================
 
 extensions = [
+    "sphinxcontrib.jquery",
     "myst_parser",
     "sphinx_copybutton",
     "sphinx_design",
     "sphinxcontrib.mermaid",
     "sphinxext.opengraph",
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.ifconfig",
     "sphinx-prompt",
+    "sphinxcontrib.redoc",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
     "sphinx_automodapi.automodapi",
     "sphinx_automodapi.smart_resolver",
     "documenteer.sphinxext",
+    "documenteer.ext.openapi",
 ]
 _conf.append_extensions(extensions)
 
 # ============================================================================
 # #SPHINX Core Sphinx configurations
 # ============================================================================
 
@@ -152,15 +162,25 @@
 
 root_doc = "index"
 
 language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ["_build", "README.rst", "README.md"]
+exclude_patterns = [
+    "_build",
+    "README.rst",
+    "README.md",
+    ".venv",
+    "venv",
+    "requirements.txt",
+    ".github",
+    ".tox",
+]
+_conf.extend_exclude_patterns(exclude_patterns)
 
 if _conf.rst_epilog_path:
     exclude_patterns.append(str(_conf.rst_epilog_path))
 
 # The reST default role cross-links Python (used for this markup: `text`)
 default_role = "py:obj"
 
@@ -358,7 +378,43 @@
 # https://github.com/wpilibsuite/sphinxext-opengraph
 # https://ogp.me/
 # ============================================================================
 
 ogp_site_url = _conf.base_url
 ogp_site_name = _conf.project
 ogp_use_first_image = True
+
+# ============================================================================
+# #OPEN OpenAPI/Redoc support
+# https://sphinxcontrib-redoc.readthedocs.io/en/stable/
+# documenteer.ext.openapi
+# ============================================================================
+
+if _conf.conf.project.openapi is not None:
+    if _conf.conf.project.openapi.generator is not None:
+        documenteer_openapi_generator: Optional[Dict[str, Any]] = {
+            "func": _conf.conf.project.openapi.generator.function,
+            "args": _conf.conf.project.openapi.generator.positional_args,
+            "kwargs": _conf.conf.project.openapi.generator.keyword_args,
+        }
+    else:
+        documenteer_openapi_generator = None
+    documenteer_openapi_path: Optional[
+        str
+    ] = _conf.conf.project.openapi.openapi_path
+    redoc: Optional[List[Any]] = [
+        {
+            "name": "REST API",
+            "page": _conf.conf.project.openapi.doc_path,
+            "spec": _conf.conf.project.openapi.openapi_path,
+            "embed": True,
+            "opts": {"hide-hostname": True},
+        }
+    ]
+    redoc_uri: Optional[
+        str
+    ] = "https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js"
+else:
+    documenteer_openapi_generator = None
+    documenteer_openapi_path = None
+    redoc = []
+    redoc_uri = None
```

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/pipelines.py` & `documenteer-1.0.0a1/src/documenteer/conf/pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     if get_package_version_semver("sphinx-jinja") < Semver.parse("2.0.0"):
         # Use older sphinx jinja name for sphinx-jinja < 2.0.0
         _sphinx_jinja_ext_name = "sphinxcontrib.jinja"
 except Exception as e:
     print(f"Error getting sphinx-jinja version: {str(e)}")
 
 extensions = [
+    "sphinxcontrib.jquery",
     "sphinx.ext.autodoc",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
     "sphinx.ext.mathjax",
     "sphinx.ext.ifconfig",
```

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/pipelinespkg.py` & `documenteer-1.0.0a1/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/technote.py` & `documenteer-1.0.0a1/src/documenteer/conf/technote.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/conf/technotebeta.py` & `documenteer-1.0.0a1/src/documenteer/conf/technotebeta.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/ext/autocppapi.py` & `documenteer-1.0.0a1/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/ext/autodocreset.py` & `documenteer-1.0.0a1/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/packagemetadata.py` & `documenteer-1.0.0a1/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/requestsutils.py` & `documenteer-1.0.0a1/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxconfig/stackconf.py` & `documenteer-1.0.0a1/src/documenteer/sphinxconfig/stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxconfig/technoteconf.py` & `documenteer-1.0.0a1/src/documenteer/sphinxconfig/technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxconfig/utils.py` & `documenteer-1.0.0a1/src/documenteer/sphinxconfig/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/__init__.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/bibtex.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/jira.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lsstdocushare.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/__init__.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/configfieldlists.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/crossrefs.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/pyapisummary.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/pyapisummary.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/taskutils.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topiclists.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topics.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/mockcoderefs.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/packagetoctree.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/remotecodeblock.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxext/utils.py` & `documenteer-1.0.0a1/src/documenteer/sphinxext/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/sphinxrunner.py` & `documenteer-1.0.0a1/src/documenteer/sphinxrunner.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/build.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/build.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-1.0.0a1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-1.0.0a1/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/doxygen.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/doxygentag.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/packagecli.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/packagecli.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/stackdocs/stackcli.py` & `documenteer-1.0.0a1/src/documenteer/stackdocs/stackcli.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/templates/technote/sections/header-article.html` & `documenteer-1.0.0a1/src/documenteer/templates/technote/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/utils.py` & `documenteer-1.0.0a1/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer/version.py` & `documenteer-1.0.0a1/src/documenteer/version.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/src/documenteer.egg-info/PKG-INFO` & `documenteer-1.0.0a1/src/documenteer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 0.8.0b2
+Version: 1.0.0a1
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-0.8.0b2/src/documenteer.egg-info/SOURCES.txt` & `documenteer-1.0.0a1/src/documenteer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 docs/dev/api/index.rst
 docs/guides/badges.rst
 docs/guides/configuration-preset.rst
 docs/guides/configuration.rst
 docs/guides/diagrams.rst
 docs/guides/extend-conf-py.rst
 docs/guides/index.rst
+docs/guides/openapi.rst
 docs/guides/organization.rst
 docs/guides/overview.rst
 docs/guides/pyproject-configuration.rst
 docs/guides/rst-epilog.rst
 docs/guides/tabsets.rst
 docs/guides/toml-reference.rst
 docs/pipelines/build-overview.rst
@@ -71,14 +72,15 @@
 docs/sphinx-extensions/autocppapi.rst
 docs/sphinx-extensions/autodocreset.rst
 docs/sphinx-extensions/docushare-reference.rst
 docs/sphinx-extensions/index.rst
 docs/sphinx-extensions/jira-reference.rst
 docs/sphinx-extensions/lsst-pybtex-style.rst
 docs/sphinx-extensions/lssttasks.rst
+docs/sphinx-extensions/openapi.rst
 docs/sphinx-extensions/package-toctree.rst
 docs/sphinx-extensions/remote-code-block.rst
 docs/technotes/configuration.rst
 docs/technotes/index.rst
 docs/technotes/refresh-lsst-bib.rst
 licenses/README.md
 licenses/astropy-helpers.txt
@@ -126,14 +128,15 @@
 src/documenteer/conf/pipelines.py
 src/documenteer/conf/pipelinespkg.py
 src/documenteer/conf/technote.py
 src/documenteer/conf/technotebeta.py
 src/documenteer/ext/__init__.py
 src/documenteer/ext/autocppapi.py
 src/documenteer/ext/autodocreset.py
+src/documenteer/ext/openapi.py
 src/documenteer/sphinxconfig/__init__.py
 src/documenteer/sphinxconfig/stackconf.py
 src/documenteer/sphinxconfig/technoteconf.py
 src/documenteer/sphinxconfig/utils.py
 src/documenteer/sphinxext/__init__.py
 src/documenteer/sphinxext/bibtex.py
 src/documenteer/sphinxext/jira.py
```

### Comparing `documenteer-0.8.0b2/src/documenteer.egg-info/requires.txt` & `documenteer-1.0.0a1/src/documenteer.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -34,22 +34,25 @@
 sphinx-automodapi
 sphinx-copybutton
 sphinx-prompt
 myst-parser
 markdown-it-py[linkify]
 sphinxcontrib-mermaid
 sphinxext-opengraph
+sphinxcontrib-redoc
+sphinxcontrib-jquery
 
 [pipelines]
 lsst-sphinx-bootstrap-theme<0.3.0,>=0.2.0
 numpydoc
 sphinx-automodapi
 sphinx-jinja
 sphinxcontrib-autoprogram
 sphinx-prompt
 sphinxcontrib-doxylink
 sphinx-click
+sphinxcontrib-jquery
 
 [technote]
 lsst-dd-rtd-theme<0.3.0,>=0.2.3
 technote>=0.2.0
 sphinx-prompt
```

### Comparing `documenteer-0.8.0b2/tests/conftest.py` & `documenteer-1.0.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/data/afw.doxygen.conf` & `documenteer-1.0.0a1/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/data/doxygen.tag.zip` & `documenteer-1.0.0a1/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/roots/test-autocppapi/conf.py` & `documenteer-1.0.0a1/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-1.0.0a1/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_conf_toml.py` & `documenteer-1.0.0a1/tests/test_conf_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_conf_utils.py` & `documenteer-1.0.0a1/tests/test_conf_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_ext_autocppapi.py` & `documenteer-1.0.0a1/tests/test_ext_autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_packagemetadata.py` & `documenteer-1.0.0a1/tests/test_packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_refreshlsstbib.py` & `documenteer-1.0.0a1/tests/test_refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxconfig_stackconf.py` & `documenteer-1.0.0a1/tests/test_sphinxconfig_stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxconfig_utils.py` & `documenteer-1.0.0a1/tests/test_sphinxconfig_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxext_jira.py` & `documenteer-1.0.0a1/tests/test_sphinxext_jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxext_lsstdocushare.py` & `documenteer-1.0.0a1/tests/test_sphinxext_lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxext_lssttasks_taskutils.py` & `documenteer-1.0.0a1/tests/test_sphinxext_lssttasks_taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxext_mockcoderefs.py` & `documenteer-1.0.0a1/tests/test_sphinxext_mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxext_packagetoctree.py` & `documenteer-1.0.0a1/tests/test_sphinxext_packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_sphinxext_utils.py` & `documenteer-1.0.0a1/tests/test_sphinxext_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_stackdocs_build.py` & `documenteer-1.0.0a1/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_stackdocs_doxygen.py` & `documenteer-1.0.0a1/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_stackdocs_doxygentag.py` & `documenteer-1.0.0a1/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-1.0.0a1/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_stackdocs_rootdiscovery.py` & `documenteer-1.0.0a1/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tests/test_technoteconf.py` & `documenteer-1.0.0a1/tests/test_technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/tox.ini` & `documenteer-1.0.0a1/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b2/webpack.config.js` & `documenteer-1.0.0a1/webpack.config.js`

 * *Files identical despite different names*

