# Comparing `tmp/collective.glossary-2.0.2.dev0.tar.gz` & `tmp/collective.glossary-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.glossary-2.0.2.dev0.tar", last modified: Thu Jul 28 07:07:27 2022, max compression
+gzip compressed data, was "collective.glossary-2.0.3.tar", last modified: Fri Jun 23 20:23:17 2023, max compression
```

## Comparing `collective.glossary-2.0.2.dev0.tar` & `collective.glossary-2.0.3.tar`

### file list

```diff
@@ -1,143 +1,128 @@
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.419376 collective.glossary-2.0.2.dev0/
--rw-r--r--   0 katjasuss   (501) staff       (20)  2760704 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/.coverage
--rw-r--r--   0 katjasuss   (501) staff       (20)       76 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/.coveragerc
--rw-r--r--   0 katjasuss   (501) staff       (20)      245 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/.editorconfig
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.386654 collective.glossary-2.0.2.dev0/.github/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.399651 collective.glossary-2.0.2.dev0/.github/workflows/
--rw-r--r--   0 katjasuss   (501) staff       (20)      794 2022-07-27 06:56:46.000000 collective.glossary-2.0.2.dev0/.github/workflows/black.yml
--rw-r--r--   0 katjasuss   (501) staff       (20)      793 2022-07-27 06:56:46.000000 collective.glossary-2.0.2.dev0/.github/workflows/flake8.yml
--rw-r--r--   0 katjasuss   (501) staff       (20)      874 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/.github/workflows/tests.yml
--rw-r--r--   0 katjasuss   (501) staff       (20)      249 2022-07-27 06:56:46.000000 collective.glossary-2.0.2.dev0/.gitignore
--rw-r--r--   0 katjasuss   (501) staff       (20)     2213 2022-07-28 06:50:02.000000 collective.glossary-2.0.2.dev0/CHANGES.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      204 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/CONTRIBUTORS.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      242 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/DEVELOP.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)    18092 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/LICENSE.GPL
--rw-r--r--   0 katjasuss   (501) staff       (20)      666 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/LICENSE.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)      460 2022-07-27 17:39:22.000000 collective.glossary-2.0.2.dev0/MANIFEST.in
--rw-r--r--   0 katjasuss   (501) staff       (20)     5723 2022-07-28 07:07:27.419496 collective.glossary-2.0.2.dev0/PKG-INFO
--rw-r--r--   0 katjasuss   (501) staff       (20)     2146 2022-07-28 06:39:30.000000 collective.glossary-2.0.2.dev0/README.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)     2186 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/base.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)       81 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/bobtemplate.cfg
--rwxr-xr-x   0 katjasuss   (501) staff       (20)      316 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/bootstrap.sh
--rw-r--r--   0 katjasuss   (501) staff       (20)       96 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/buildout.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)       27 2022-07-27 17:34:16.000000 collective.glossary-2.0.2.dev0/constraints.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       62 2022-07-27 17:34:16.000000 collective.glossary-2.0.2.dev0/constraints_plone60.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)    11162 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/coverage.xml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.401484 collective.glossary-2.0.2.dev0/docs/
--rw-r--r--   0 katjasuss   (501) staff       (20)     7897 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/docs/conf.py
--rw-r--r--   0 katjasuss   (501) staff       (20)    29428 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/docs/controlpanel.png
--rw-r--r--   0 katjasuss   (501) staff       (20)   111592 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/docs/glossary.png
--rw-r--r--   0 katjasuss   (501) staff       (20)       80 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/docs/index.rst
--rw-r--r--   0 katjasuss   (501) staff       (20)    73512 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/docs/usage.png
--rw-r--r--   0 katjasuss   (501) staff       (20)      123 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/requirements.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)      123 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/requirements_52.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)      518 2022-07-28 07:07:27.419993 collective.glossary-2.0.2.dev0/setup.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)     2605 2022-07-28 06:50:02.000000 collective.glossary-2.0.2.dev0/setup.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.386933 collective.glossary-2.0.2.dev0/src/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.401746 collective.glossary-2.0.2.dev0/src/collective/
--rw-r--r--   0 katjasuss   (501) staff       (20)       80 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.406248 collective.glossary-2.0.2.dev0/src/collective/glossary/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.406771 collective.glossary-2.0.2.dev0/src/collective/glossary/Extensions/
--rw-r--r--   0 katjasuss   (501) staff       (20)      379 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/Extensions/Install.py
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/Extensions/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      114 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/__init__.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.407288 collective.glossary-2.0.2.dev0/src/collective/glossary/api/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      241 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.407574 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      241 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.408006 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/glossary/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/glossary/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      507 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/glossary/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)     3351 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/glossary/get.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.408677 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1580 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.410287 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/
--rw-r--r--   0 katjasuss   (501) staff       (20)      376 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/glossary-icon.png
--rw-r--r--   0 katjasuss   (501) staff       (20)     7974 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/jquery.glossarize.js
--rw-r--r--   0 katjasuss   (501) staff       (20)     1656 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/main.css
--rw-r--r--   0 katjasuss   (501) staff       (20)      422 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/main.js
--rw-r--r--   0 katjasuss   (501) staff       (20)      626 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/term-icon.png
--rw-r--r--   0 katjasuss   (501) staff       (20)     1262 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/tooltip.css
--rw-r--r--   0 katjasuss   (501) staff       (20)     2821 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/tooltip.js
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.410576 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/templates/
--rw-r--r--   0 katjasuss   (501) staff       (20)     2451 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/templates/glossary.pt
--rw-r--r--   0 katjasuss   (501) staff       (20)     1195 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/templates/term.pt
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.411271 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      702 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)      833 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/css_js.pt
--rw-r--r--   0 katjasuss   (501) staff       (20)      207 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/viewlets.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     5022 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/browser/views.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      242 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/config.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      878 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)      335 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/content.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      550 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/controlpanel.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      303 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/indexers.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     2393 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/interfaces.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.412188 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/
--rw-r--r--   0 katjasuss   (501) staff       (20)      689 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/README.md
--rw-r--r--   0 katjasuss   (501) staff       (20)     2107 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/collective.glossary.pot
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.387810 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/de/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.412395 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/de/LC_MESSAGES/
--rw-r--r--   0 katjasuss   (501) staff       (20)     2245 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/de/LC_MESSAGES/collective.glossary.po
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.387945 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/en/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.412546 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/en/LC_MESSAGES/
--rw-r--r--   0 katjasuss   (501) staff       (20)     1998 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/en/LC_MESSAGES/collective.glossary.po
--rw-r--r--   0 katjasuss   (501) staff       (20)     1749 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/update.py
--rwxr-xr-x   0 katjasuss   (501) staff       (20)      493 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/locales/update.sh
--rw-r--r--   0 katjasuss   (501) staff       (20)      133 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/logger.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.388222 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.413846 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/
--rw-r--r--   0 katjasuss   (501) staff       (20)      156 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/browserlayer.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      127 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/catalog.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      575 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/controlpanel.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      232 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/metadata.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      120 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/registry.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      512 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/rolemap.xml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.414142 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/types/
--rw-r--r--   0 katjasuss   (501) staff       (20)     1942 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/types/Glossary.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)     1839 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/types/Term.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)      196 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/types.xml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.414296 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/uninstall/
--rw-r--r--   0 katjasuss   (501) staff       (20)      134 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/uninstall/registry.xml
--rw-r--r--   0 katjasuss   (501) staff       (20)     1000 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/profiles.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)      396 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/setuphandlers.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1371 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/testing.py
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.417905 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     2082 2022-07-27 21:27:56.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_controlpanel.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1512 2022-07-27 21:27:56.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_glossary.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      595 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_robot.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1387 2022-07-27 21:27:56.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_term.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     7432 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_views.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1480 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/tests/todo_test_glossary.robot
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.418206 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/
--rw-r--r--   0 katjasuss   (501) staff       (20)       24 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      151 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.418566 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2/
--rw-r--r--   0 katjasuss   (501) staff       (20)     1216 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)     1158 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.418913 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2a/
--rw-r--r--   0 katjasuss   (501) staff       (20)     1043 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2a/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      529 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2a/configure.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.419234 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2b/
--rw-r--r--   0 katjasuss   (501) staff       (20)      420 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2b/__init__.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      485 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2b/configure.zcml
--rw-r--r--   0 katjasuss   (501) staff       (20)      317 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/utils.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      639 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/vocabulary.py
--rw-r--r--   0 katjasuss   (501) staff       (20)      250 2022-07-27 05:37:10.000000 collective.glossary-2.0.2.dev0/src/collective/glossary/vocabulary.zcml
-drwxr-xr-x   0 katjasuss   (501) staff       (20)        0 2022-07-28 07:07:27.403084 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/
--rw-r--r--   0 katjasuss   (501) staff       (20)     5723 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/PKG-INFO
--rw-r--r--   0 katjasuss   (501) staff       (20)     4293 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/SOURCES.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)        1 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/dependency_links.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)      144 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/entry_points.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       11 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/namespace_packages.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)        1 2022-07-27 05:37:11.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/not-zip-safe
--rw-r--r--   0 katjasuss   (501) staff       (20)      241 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/requires.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)       11 2022-07-28 07:07:27.000000 collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/top_level.txt
--rw-r--r--   0 katjasuss   (501) staff       (20)      268 2022-07-27 17:34:16.000000 collective.glossary-2.0.2.dev0/test_plone52.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)      747 2022-07-28 05:58:08.000000 collective.glossary-2.0.2.dev0/test_plone60.cfg
--rw-r--r--   0 katjasuss   (501) staff       (20)     3152 2022-07-28 05:42:16.000000 collective.glossary-2.0.2.dev0/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.859953 collective.glossary-2.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     2325 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      204 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      242 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/DEVELOP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      666 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      490 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     6037 2023-06-23 20:23:17.860056 collective.glossary-2.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2265 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/README.rst
+-rwxr-xr-x   0 maurits    (501) staff       (20)      316 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/bootstrap.sh
+-rw-r--r--   0 maurits    (501) staff       (20)       27 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/constraints.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       62 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/constraints_plone60.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.832351 collective.glossary-2.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     7897 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29428 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/docs/controlpanel.png
+-rw-r--r--   0 maurits    (501) staff       (20)   111592 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/docs/glossary.png
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    73512 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/docs/usage.png
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/requirements_52.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      518 2023-06-23 20:23:17.860581 collective.glossary-2.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2706 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.821590 collective.glossary-2.0.3/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.832909 collective.glossary-2.0.3/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.840982 collective.glossary-2.0.3/src/collective/glossary/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.841716 collective.glossary-2.0.3/src/collective/glossary/Extensions/
+-rw-r--r--   0 maurits    (501) staff       (20)      379 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/Extensions/Install.py
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/Extensions/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      114 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.842567 collective.glossary-2.0.3/src/collective/glossary/api/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.843206 collective.glossary-2.0.3/src/collective/glossary/api/services/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/services/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/services/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.844240 collective.glossary-2.0.3/src/collective/glossary/api/services/glossary/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/services/glossary/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      507 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/services/glossary/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3351 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/api/services/glossary/get.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.845301 collective.glossary-2.0.3/src/collective/glossary/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1580 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.847622 collective.glossary-2.0.3/src/collective/glossary/browser/static/
+-rw-r--r--   0 maurits    (501) staff       (20)      376 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/glossary-icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)     7974 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/jquery.glossarize.js
+-rw-r--r--   0 maurits    (501) staff       (20)     1656 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/main.css
+-rw-r--r--   0 maurits    (501) staff       (20)      422 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/main.js
+-rw-r--r--   0 maurits    (501) staff       (20)      626 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/term-icon.png
+-rw-r--r--   0 maurits    (501) staff       (20)     1262 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/tooltip.css
+-rw-r--r--   0 maurits    (501) staff       (20)     2821 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/static/tooltip.js
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.848294 collective.glossary-2.0.3/src/collective/glossary/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     2451 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/templates/glossary.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1195 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/templates/term.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.849635 collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      702 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      833 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/css_js.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      207 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/viewlets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5229 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/browser/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)      242 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)      878 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      335 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/indexers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2393 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.850998 collective.glossary-2.0.3/src/collective/glossary/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)      689 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/locales/README.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2107 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/locales/collective.glossary.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.823859 collective.glossary-2.0.3/src/collective/glossary/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.851299 collective.glossary-2.0.3/src/collective/glossary/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     2245 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/locales/de/LC_MESSAGES/collective.glossary.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.824293 collective.glossary-2.0.3/src/collective/glossary/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.851565 collective.glossary-2.0.3/src/collective/glossary/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)     1998 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/locales/en/LC_MESSAGES/collective.glossary.po
+-rw-r--r--   0 maurits    (501) staff       (20)     1749 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/locales/update.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)      493 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/locales/update.sh
+-rw-r--r--   0 maurits    (501) staff       (20)      133 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/logger.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.824914 collective.glossary-2.0.3/src/collective/glossary/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.853503 collective.glossary-2.0.3/src/collective/glossary/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      156 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/catalog.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      575 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      232 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      120 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      512 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.854092 collective.glossary-2.0.3/src/collective/glossary/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     1942 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/types/Glossary.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1839 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/types/Term.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      196 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.854352 collective.glossary-2.0.3/src/collective/glossary/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      134 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      396 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1370 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.857090 collective.glossary-2.0.3/src/collective/glossary/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2080 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/test_controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1511 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/test_glossary.py
+-rw-r--r--   0 maurits    (501) staff       (20)      595 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1386 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/test_term.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7431 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/test_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1480 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/tests/todo_test_glossary.robot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.857713 collective.glossary-2.0.3/src/collective/glossary/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)       24 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      151 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.858438 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2/
+-rw-r--r--   0 maurits    (501) staff       (20)     1216 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1158 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.859017 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2a/
+-rw-r--r--   0 maurits    (501) staff       (20)     1043 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2a/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      529 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2a/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.859580 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2b/
+-rw-r--r--   0 maurits    (501) staff       (20)      420 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2b/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      485 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/upgrades/v2b/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      317 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      639 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/vocabulary.py
+-rw-r--r--   0 maurits    (501) staff       (20)      250 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective/glossary/vocabulary.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-23 20:23:17.835783 collective.glossary-2.0.3/src/collective.glossary.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     6037 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4076 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      124 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/src/collective.glossary.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3072 2023-06-23 20:23:17.000000 collective.glossary-2.0.3/tox.ini
```

### Comparing `collective.glossary-2.0.2.dev0/CHANGES.rst` & `collective.glossary-2.0.3/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Changelog
 =========
 
 
-2.0.2 (unreleased)
+2.0.3 (2023-06-23)
 ------------------
 
-- Nothing changed yet.
+- Speed up glossary view by getting the entries only once.  [maurits]
+
+
+2.0.2 (2022-07-28)
+------------------
+
+- Link to Support page.
 
 
 2.0.1 (2022-07-28)
 ------------------
 
 - Add restapi services to fetch glossary terms and settings. @ksuess
 - Replace term description by richtext definition. @ksuess
```

### Comparing `collective.glossary-2.0.2.dev0/LICENSE.GPL` & `collective.glossary-2.0.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/LICENSE.rst` & `collective.glossary-2.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/PKG-INFO` & `collective.glossary-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: collective.glossary
-Version: 2.0.2.dev0
+Version: 2.0.3
 Summary: Content types to define a glossary and its terms
 Home-page: https://github.com/collective/collective.glossary
 Author: Simples Consultoria
 Author-email: products@simplesconsultoria.com.br
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.glossary
 Project-URL: Source, https://github.com/collective/collective.glossary
 Project-URL: Tracker, https://github.com/collective/collective.glossary/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
@@ -85,14 +86,20 @@
 ----------
 
 - Issue Tracker: https://github.com/collective/collective.glossary/issues
 - Source Code: https://github.com/collective/collective.glossary
 - Documentation: https://docs.plone.org/foo/bar
 
 
+Support
+-------
+
+If you are having issues, please let us know: `community.plone.org <https://community.plone.org/>`_
+
+
 License
 -------
 
 The project is licensed under the GPLv2.
 
 
 
@@ -123,18 +130,24 @@
 - Katja Süss, Rohberg, @ksuess
 
 
 Changelog
 =========
 
 
-2.0.2 (unreleased)
+2.0.3 (2023-06-23)
+------------------
+
+- Speed up glossary view by getting the entries only once.  [maurits]
+
+
+2.0.2 (2022-07-28)
 ------------------
 
-- Nothing changed yet.
+- Link to Support page.
 
 
 2.0.1 (2022-07-28)
 ------------------
 
 - Add restapi services to fetch glossary terms and settings. @ksuess
 - Replace term description by richtext definition. @ksuess
@@ -212,9 +225,7 @@
 .. _`#5`: https://github.com/collective/collective.cover/issues/5
 .. _`#8`: https://github.com/collective/collective.cover/issues/8
 .. _`#12`: https://github.com/collective/collective.cover/issues/12
 .. _`#14`: https://github.com/collective/collective.cover/issues/14
 .. _`#18`: https://github.com/collective/collective.cover/issues/18
 .. _`#22`: https://github.com/collective/collective.cover/issues/22
 .. _`#26`: https://github.com/collective/collective.cover/issues/26
-
-
```

### Comparing `collective.glossary-2.0.2.dev0/README.rst` & `collective.glossary-2.0.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 ----------
 
 - Issue Tracker: https://github.com/collective/collective.glossary/issues
 - Source Code: https://github.com/collective/collective.glossary
 - Documentation: https://docs.plone.org/foo/bar
 
 
+Support
+-------
+
+If you are having issues, please let us know: `community.plone.org <https://community.plone.org/>`_
+
+
 License
 -------
 
 The project is licensed under the GPLv2.
```

### Comparing `collective.glossary-2.0.2.dev0/docs/conf.py` & `collective.glossary-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/docs/controlpanel.png` & `collective.glossary-2.0.3/docs/controlpanel.png`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/docs/glossary.png` & `collective.glossary-2.0.3/docs/glossary.png`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/docs/usage.png` & `collective.glossary-2.0.3/docs/usage.png`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/setup.cfg` & `collective.glossary-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/setup.py` & `collective.glossary-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,30 @@
         open("CONTRIBUTORS.rst").read(),
         open("CHANGES.rst").read(),
     ]
 )
 
 setup(
     name="collective.glossary",
-    version="2.0.2.dev0",
+    version="2.0.3",
     description="Content types to define a glossary and its terms",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
         "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     keywords="Python Plone CMS",
     author="Simples Consultoria",
     author_email="products@simplesconsultoria.com.br",
     url="https://github.com/collective/collective.glossary",
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/api/services/glossary/get.py` & `collective.glossary-2.0.3/src/collective/glossary/api/services/glossary/get.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/configure.zcml` & `collective.glossary-2.0.3/src/collective/glossary/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/jquery.glossarize.js` & `collective.glossary-2.0.3/src/collective/glossary/browser/static/jquery.glossarize.js`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/main.css` & `collective.glossary-2.0.3/src/collective/glossary/browser/static/main.css`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/term-icon.png` & `collective.glossary-2.0.3/src/collective/glossary/browser/static/term-icon.png`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/tooltip.css` & `collective.glossary-2.0.3/src/collective/glossary/browser/static/tooltip.css`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/static/tooltip.js` & `collective.glossary-2.0.3/src/collective/glossary/browser/static/tooltip.js`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/templates/glossary.pt` & `collective.glossary-2.0.3/src/collective/glossary/browser/templates/glossary.pt`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/templates/term.pt` & `collective.glossary-2.0.3/src/collective/glossary/browser/templates/term.pt`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/configure.zcml` & `collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/viewlets/css_js.pt` & `collective.glossary-2.0.3/src/collective/glossary/browser/viewlets/css_js.pt`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/browser/views.py` & `collective.glossary-2.0.3/src/collective/glossary/browser/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 class TermView(BrowserView):
     """Default view for Term type"""
 
 
 class GlossaryView(BrowserView):
     """Default view of Glossary type"""
 
-    def get_entries(self):
+    def _get_entries(self):
         """Get glossary entries and keep them in the desired format"""
-
         catalog = api.portal.get_tool("portal_catalog")
         path = "/".join(self.context.getPhysicalPath())
         query = dict(portal_type="Term", path={"query": path, "depth": 1})
 
         items = defaultdict(list)
         for brain in catalog(**query):
             obj = brain.getObject()
@@ -42,14 +41,21 @@
         for k in items:
             items[k] = sorted(
                 items[k],
                 key=lambda term: term["title"],
             )
         return items
 
+    def get_entries(self):
+        entries = getattr(self, "_entries", None)
+        if entries is None:
+            entries = self._get_entries()
+            self._entries = entries
+        return entries
+
     def letters(self):
         """Return all letters sorted"""
 
         return sorted(self.get_entries())
 
     def terms(self, letter):
         """Return all terms of one letter"""
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/configure.zcml` & `collective.glossary-2.0.3/src/collective/glossary/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/controlpanel.py` & `collective.glossary-2.0.3/src/collective/glossary/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/interfaces.py` & `collective.glossary-2.0.3/src/collective/glossary/interfaces.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/locales/README.md` & `collective.glossary-2.0.3/src/collective/glossary/locales/README.md`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/locales/collective.glossary.pot` & `collective.glossary-2.0.3/src/collective/glossary/locales/collective.glossary.pot`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/locales/de/LC_MESSAGES/collective.glossary.po` & `collective.glossary-2.0.3/src/collective/glossary/locales/de/LC_MESSAGES/collective.glossary.po`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/locales/en/LC_MESSAGES/collective.glossary.po` & `collective.glossary-2.0.3/src/collective/glossary/locales/en/LC_MESSAGES/collective.glossary.po`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/locales/update.py` & `collective.glossary-2.0.3/src/collective/glossary/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/controlpanel.xml` & `collective.glossary-2.0.3/src/collective/glossary/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/rolemap.xml` & `collective.glossary-2.0.3/src/collective/glossary/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/types/Glossary.xml` & `collective.glossary-2.0.3/src/collective/glossary/profiles/default/types/Glossary.xml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/profiles/default/types/Term.xml` & `collective.glossary-2.0.3/src/collective/glossary/profiles/default/types/Term.xml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/profiles.zcml` & `collective.glossary-2.0.3/src/collective/glossary/profiles.zcml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/testing.py` & `collective.glossary-2.0.3/src/collective/glossary/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         PLONE_APP_CONTENTTYPES_FIXTURE as PLONE_FIXTURE,
     )
 
 IS_PLONE_5 = api.env.plone_version().startswith("5")
 
 
 class Fixture(PloneSandboxLayer):
-
     defaultBases = (PLONE_FIXTURE,)
 
     def setUpZope(self, app, configurationContext):
         import collective.glossary
 
         self.loadZCML(package=collective.glossary)
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_controlpanel.py` & `collective.glossary-2.0.3/src/collective/glossary/tests/test_controlpanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from zope.component import getMultiAdapter, getUtility
 from zope.interface import alsoProvides
 
 import unittest
 
 
 class ControlPanelTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         alsoProvides(self.request, IGlossaryLayer)
         self.controlpanel = self.portal["portal_controlpanel"]
@@ -35,15 +34,14 @@
 
     def test_controlpanel_installed(self):
         actions = [a.getAction(self)["id"] for a in self.controlpanel.listActions()]
         self.assertIn("glossary", actions)
 
 
 class RegistryTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
         self.registry = getUtility(IRegistry)
         self.settings = self.registry.forInterface(IGlossarySettings)  # noqa: P001
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_glossary.py` & `collective.glossary-2.0.3/src/collective/glossary/tests/test_glossary.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from plone.dexterity.interfaces import IDexterityFTI
 from zope.component import createObject, queryUtility
 
 import unittest
 
 
 class GlossaryTypeTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
 
         with api.env.adopt_roles(["Manager"]):
             self.g1 = api.content.create(self.portal, "Glossary", "g1")
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_robot.py` & `collective.glossary-2.0.3/src/collective/glossary/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_term.py` & `collective.glossary-2.0.3/src/collective/glossary/tests/test_term.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from plone.dexterity.interfaces import IDexterityFTI
 from zope.component import createObject, queryUtility
 
 import unittest
 
 
 class GlossaryTypeTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.portal = self.layer["portal"]
 
         with api.env.adopt_roles(["Manager"]):
             self.g1 = api.content.create(self.portal, "Glossary", "g1")
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/tests/test_views.py` & `collective.glossary-2.0.3/src/collective/glossary/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from plone.app.textfield.value import RichTextValue
 from zope.publisher.browser import TestRequest
 
 import unittest
 
 
 class BaseViewTestCase(unittest.TestCase):
-
     layer = INTEGRATION_TESTING
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/tests/todo_test_glossary.robot` & `collective.glossary-2.0.3/src/collective/glossary/tests/todo_test_glossary.robot`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2/__init__.py` & `collective.glossary-2.0.3/src/collective/glossary/upgrades/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2/configure.zcml` & `collective.glossary-2.0.3/src/collective/glossary/upgrades/v2/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2a/__init__.py` & `collective.glossary-2.0.3/src/collective/glossary/upgrades/v2a/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/upgrades/v2a/configure.zcml` & `collective.glossary-2.0.3/src/collective/glossary/upgrades/v2a/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective/glossary/vocabulary.py` & `collective.glossary-2.0.3/src/collective/glossary/vocabulary.py`

 * *Files identical despite different names*

### Comparing `collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/PKG-INFO` & `collective.glossary-2.0.3/src/collective.glossary.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: collective.glossary
-Version: 2.0.2.dev0
+Version: 2.0.3
 Summary: Content types to define a glossary and its terms
 Home-page: https://github.com/collective/collective.glossary
 Author: Simples Consultoria
 Author-email: products@simplesconsultoria.com.br
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.glossary
 Project-URL: Source, https://github.com/collective/collective.glossary
 Project-URL: Tracker, https://github.com/collective/collective.glossary/issues
 Keywords: Python Plone CMS
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.7
 Provides-Extra: test
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 
@@ -85,14 +86,20 @@
 ----------
 
 - Issue Tracker: https://github.com/collective/collective.glossary/issues
 - Source Code: https://github.com/collective/collective.glossary
 - Documentation: https://docs.plone.org/foo/bar
 
 
+Support
+-------
+
+If you are having issues, please let us know: `community.plone.org <https://community.plone.org/>`_
+
+
 License
 -------
 
 The project is licensed under the GPLv2.
 
 
 
@@ -123,18 +130,24 @@
 - Katja Süss, Rohberg, @ksuess
 
 
 Changelog
 =========
 
 
-2.0.2 (unreleased)
+2.0.3 (2023-06-23)
+------------------
+
+- Speed up glossary view by getting the entries only once.  [maurits]
+
+
+2.0.2 (2022-07-28)
 ------------------
 
-- Nothing changed yet.
+- Link to Support page.
 
 
 2.0.1 (2022-07-28)
 ------------------
 
 - Add restapi services to fetch glossary terms and settings. @ksuess
 - Replace term description by richtext definition. @ksuess
@@ -212,9 +225,7 @@
 .. _`#5`: https://github.com/collective/collective.cover/issues/5
 .. _`#8`: https://github.com/collective/collective.cover/issues/8
 .. _`#12`: https://github.com/collective/collective.cover/issues/12
 .. _`#14`: https://github.com/collective/collective.cover/issues/14
 .. _`#18`: https://github.com/collective/collective.cover/issues/18
 .. _`#22`: https://github.com/collective/collective.cover/issues/22
 .. _`#26`: https://github.com/collective/collective.cover/issues/26
-
-
```

### Comparing `collective.glossary-2.0.2.dev0/src/collective.glossary.egg-info/SOURCES.txt` & `collective.glossary-2.0.3/src/collective.glossary.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-.coverage
-.coveragerc
-.editorconfig
-.gitignore
 CHANGES.rst
 CONTRIBUTORS.rst
 DEVELOP.rst
 LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
-base.cfg
-bobtemplate.cfg
 bootstrap.sh
-buildout.cfg
 constraints.txt
 constraints_plone60.txt
-coverage.xml
 requirements.txt
 requirements_52.txt
 setup.cfg
 setup.py
-test_plone52.cfg
-test_plone60.cfg
 tox.ini
-.github/workflows/black.yml
-.github/workflows/flake8.yml
-.github/workflows/tests.yml
 docs/conf.py
 docs/controlpanel.png
 docs/glossary.png
 docs/index.rst
 docs/usage.png
 src/collective/__init__.py
 src/collective.glossary.egg-info/PKG-INFO
```

### Comparing `collective.glossary-2.0.2.dev0/tox.ini` & `collective.glossary-2.0.3/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 [tox]
 envlist =
     lint,
     black-check,
-    py{37,38,39}-plone60,
-    py{37,38,39}-plone52,
+    py{38,311}-plone60,
+    py{38}-plone52,
 #    docs,
     coverage-report,
 
 skip_missing_interpreters = True
 
 
 [gh-actions]
 python =
-    3.7: py37
     3.8: py38
-    3.9: py39
-
-[gh-actions:env]
-PLONE =
-    6.0: plone60
-    5.2: plone52
+    3.11: py311
 
 
 [testenv]
 skip_install = true
 
 extras =
     develop
@@ -100,15 +94,15 @@
     mkdir -p {toxinidir}/reports/flake8
     - flake8 --format=html --htmldir={toxinidir}/reports/flake8 --doctests {toxinidir}/src {toxinidir}/setup.py
     flake8 --doctests {toxinidir}/setup.py
     flake8 --doctests {toxinidir}/src
     isort --check-only {toxinidir}/src {toxinidir}/setup.py
     # black --check --diff -v {toxinidir}/src {toxinidir}/setup.py
 
-whitelist_externals =
+allowlist_externals =
     mkdir
 
 
 [testenv:isort-apply]
 skip_install = true
 
 deps =
@@ -142,15 +136,15 @@
 
 
 [testenv:lint]
 basepython = python3.9
 skip_install = true
 deps = {[lint]deps}
 commands = {[lint]commands}
-whitelist_externals = {[lint]whitelist_externals}
+allowlist_externals = {[lint]allowlist_externals}
 
 [testenv:docs]
 skip_install = true
 
 deps =
     Sphinx
```

