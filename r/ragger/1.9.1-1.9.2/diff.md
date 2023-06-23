# Comparing `tmp/ragger-1.9.1.tar.gz` & `tmp/ragger-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragger-1.9.1.tar", last modified: Thu Jun 22 16:29:25 2023, max compression
+gzip compressed data, was "ragger-1.9.2.tar", last modified: Fri Jun 23 09:11:48 2023, max compression
```

## Comparing `ragger-1.9.1.tar` & `ragger-1.9.2.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-22 16:29:13.000000 ragger-1.9.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.150336 ragger-1.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.158336 ragger-1.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/build_and_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-22 16:29:13.000000 ragger-1.9.1/.github/workflows/fast-checks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 16:29:13.000000 ragger-1.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-22 16:29:13.000000 ragger-1.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 16:29:13.000000 ragger-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 16:29:13.000000 ragger-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-06-22 16:29:25.178336 ragger-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-06-22 16:29:13.000000 ragger-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.158336 ragger-1.9.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/_static/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/navigate.draw
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/navigate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/ragger.png
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/stax_infos.png
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/stax_welcome.png
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/usage.draw
--rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/images/usage.svg
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/rationale.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/source.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial_conftest.rst
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-22 16:29:13.000000 ragger-1.9.1/doc/tutorial_screen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 16:29:13.000000 ragger-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-22 16:29:25.178336 ragger-1.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.150336 ragger-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/src/ragger/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/ledgercomm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/ledgerwallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/physical_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/speculos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/backend/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/bip/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/bip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/bip/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/bip/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/conftest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/conftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/conftest/base_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/conftest/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.166336 ragger-1.9.1/src/ragger/firmware/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/firmware/stax/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/stax/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/firmware/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanos_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanos_leftbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanos_rightbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanosp_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanosp_leftbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanosp_rightbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanox_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanox_leftbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/nanox_rightbutton.png
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/stax_body.png
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/assets/touch_action.png
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/gui/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/navigator/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/nano_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/navigator/stax_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/src/ragger/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-22 16:29:13.000000 ragger-1.9.1/src/ragger/utils/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.162336 ragger-1.9.1/src/ragger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 16:29:25.000000 ragger-1.9.1/src/ragger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/template/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 16:29:13.000000 ragger-1.9.1/template/.dispatch_to_your_test_folder
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-22 16:29:13.000000 ragger-1.9.1/template/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 16:29:13.000000 ragger-1.9.1/template/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/functional/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/backend/test_speculos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.170336 ragger-1.9.1/tests/functional/navigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/navigator/test_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/functional/test_boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.154336 ragger-1.9.1/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.154336 ragger-1.9.1/tests/snapshots/nanos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/generic/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00003.png
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/generic/00004.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00003.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00004.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00005.png
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00006.png
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare/00007.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_no_golden/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_no_golden/00000.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00001.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/nanos/test_navigate_until_text_and_compare/00003.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.154336 ragger-1.9.1/tests/snapshots/stax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/snapshots/stax/waiting_screen/
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00000.png
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00001.png
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00002.png
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00003.png
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/snapshots/stax/waiting_screen/00004.png
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_ledgercomm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_ledgerwallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_physical_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_speculos.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/backend/test_stub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/bip/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/bip/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/bip/test_seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.174336 ragger-1.9.1/tests/unit/firmware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/tests/unit/firmware/stax/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/stax/test_layouts__Layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/stax/test_screen_FullScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/stax/test_screen_MetaScreen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/test_structs_Firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/firmware/test_versions_VersionManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/tests/unit/navigator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/navigator/test_navigator.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/test_error_ApplicationError.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:25.178336 ragger-1.9.1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 16:29:13.000000 ragger-1.9.1/tests/unit/utils/test_structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-23 09:11:33.000000 ragger-1.9.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:47.999316 ragger-1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.007315 ragger-1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-06-23 09:11:33.000000 ragger-1.9.2/.github/workflows/build_and_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-23 09:11:33.000000 ragger-1.9.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-23 09:11:33.000000 ragger-1.9.2/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-23 09:11:33.000000 ragger-1.9.2/.github/workflows/fast-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-23 09:11:33.000000 ragger-1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-23 09:11:33.000000 ragger-1.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 09:11:33.000000 ragger-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 09:11:33.000000 ragger-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-06-23 09:11:48.031316 ragger-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-06-23 09:11:33.000000 ragger-1.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.011316 ragger-1.9.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.011316 ragger-1.9.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/_static/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.011316 ragger-1.9.2/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.011316 ragger-1.9.2/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/navigate.draw
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/navigate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/ragger.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/stax_infos.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/stax_welcome.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/usage.draw
+-rw-r--r--   0 runner    (1001) docker     (123)    22677 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/images/usage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/rationale.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/source.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19747 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/tutorial_conftest.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/tutorial_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-23 09:11:33.000000 ragger-1.9.2/doc/tutorial_screen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-23 09:11:33.000000 ragger-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-23 09:11:48.031316 ragger-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:47.999316 ragger-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.011316 ragger-1.9.2/src/ragger/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:11:47.000000 ragger-1.9.2/src/ragger/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.015316 ragger-1.9.2/src/ragger/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/ledgercomm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/ledgerwallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/physical_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/speculos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/backend/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.015316 ragger-1.9.2/src/ragger/bip/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/bip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/bip/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/bip/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.015316 ragger-1.9.2/src/ragger/conftest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/conftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/conftest/base_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/conftest/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.015316 ragger-1.9.2/src/ragger/firmware/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.015316 ragger-1.9.2/src/ragger/firmware/stax/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/stax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/stax/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/stax/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/stax/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/stax/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/firmware/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.015316 ragger-1.9.2/src/ragger/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.019316 ragger-1.9.2/src/ragger/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanos_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanos_leftbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanos_rightbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanosp_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanosp_leftbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanosp_rightbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanox_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanox_leftbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/nanox_rightbutton.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/stax_body.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/assets/touch_action.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/gui/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.019316 ragger-1.9.2/src/ragger/navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/navigator/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/navigator/nano_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/navigator/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/navigator/stax_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.019316 ragger-1.9.2/src/ragger/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-23 09:11:33.000000 ragger-1.9.2/src/ragger/utils/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.011316 ragger-1.9.2/src/ragger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-06-23 09:11:47.000000 ragger-1.9.2/src/ragger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-23 09:11:47.000000 ragger-1.9.2/src/ragger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:11:47.000000 ragger-1.9.2/src/ragger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-23 09:11:47.000000 ragger-1.9.2/src/ragger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 09:11:47.000000 ragger-1.9.2/src/ragger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.023316 ragger-1.9.2/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 09:11:33.000000 ragger-1.9.2/template/.dispatch_to_your_test_folder
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-23 09:11:33.000000 ragger-1.9.2/template/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-23 09:11:33.000000 ragger-1.9.2/template/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.023316 ragger-1.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.023316 ragger-1.9.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.023316 ragger-1.9.2/tests/functional/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/functional/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/functional/backend/test_speculos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.023316 ragger-1.9.2/tests/functional/navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/functional/navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/functional/navigator/test_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/functional/test_boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.003316 ragger-1.9.2/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.003316 ragger-1.9.2/tests/snapshots/nanos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.023316 ragger-1.9.2/tests/snapshots/nanos/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/generic/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/generic/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/generic/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/generic/00003.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/generic/00004.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.027316 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00003.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00004.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00005.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00006.png
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare/00007.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.027316 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare_no_golden/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare_no_golden/00000.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.027316 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_and_compare_wrong_golden/00001.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.027316 ragger-1.9.2/tests/snapshots/nanos/test_navigate_until_text_and_compare/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_until_text_and_compare/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_until_text_and_compare/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_until_text_and_compare/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/nanos/test_navigate_until_text_and_compare/00003.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.003316 ragger-1.9.2/tests/snapshots/stax/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.027316 ragger-1.9.2/tests/snapshots/stax/waiting_screen/
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/stax/waiting_screen/00000.png
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/stax/waiting_screen/00001.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/stax/waiting_screen/00002.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/stax/waiting_screen/00003.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/snapshots/stax/waiting_screen/00004.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.027316 ragger-1.9.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/tests/unit/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/test_ledgercomm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/test_ledgerwallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/test_physical_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/test_speculos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/backend/test_stub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/tests/unit/bip/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/bip/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8622 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/bip/test_seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/tests/unit/firmware/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/tests/unit/firmware/stax/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/firmware/stax/test_layouts__Layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/firmware/stax/test_screen_FullScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/firmware/stax/test_screen_MetaScreen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/firmware/test_structs_Firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/firmware/test_versions_VersionManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/tests/unit/navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/navigator/test_navigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/test_error_ApplicationError.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:48.031316 ragger-1.9.2/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/utils/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-23 09:11:33.000000 ragger-1.9.2/tests/unit/utils/test_structs.py
```

### Comparing `ragger-1.9.1/.github/workflows/build_and_tests.yml` & `ragger-1.9.2/.github/workflows/build_and_tests.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/.github/workflows/codeql-analysis.yml` & `ragger-1.9.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/.github/workflows/documentation.yml` & `ragger-1.9.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/.github/workflows/fast-checks.yml` & `ragger-1.9.2/.github/workflows/fast-checks.yml`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/CHANGELOG.md` & `ragger-1.9.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.9.2] - 2023-06-23
+
+### Fixed
+- navigator: Restore `NavInsID.USE_CASE_REVIEW_CONFIRM` custom wait for screen change for cases where the app call `io_seproxyhal_io_heartbeat()` before next screen is displayed.
+
 ## [1.9.1] - 2023-06-22
 
 ### Fixed
 - speculos: Only pause ticker during navigation steps
 
 ## [1.9.0] - 2023-06-21
```

### Comparing `ragger-1.9.1/LICENSE` & `ragger-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/PKG-INFO` & `ragger-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragger
-Version: 1.9.1
+Version: 1.9.2
 Summary: Testing framework using Speculos and LedgerComm as backends
 Home-page: https://github.com/LedgerHQ/ragger
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/ragger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ragger-1.9.1/README.md` & `ragger-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/Makefile` & `ragger-1.9.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/conf.py` & `ragger-1.9.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/faq.rst` & `ragger-1.9.2/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/glossary.rst` & `ragger-1.9.2/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/images/navigate.draw` & `ragger-1.9.2/doc/images/navigate.draw`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/images/navigate.svg` & `ragger-1.9.2/doc/images/navigate.svg`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/images/stax_infos.png` & `ragger-1.9.2/doc/images/stax_infos.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/images/stax_welcome.png` & `ragger-1.9.2/doc/images/stax_welcome.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/images/usage.draw` & `ragger-1.9.2/doc/images/usage.draw`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/images/usage.svg` & `ragger-1.9.2/doc/images/usage.svg`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/index.rst` & `ragger-1.9.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/installation.rst` & `ragger-1.9.2/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/rationale.rst` & `ragger-1.9.2/doc/rationale.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/source.rst` & `ragger-1.9.2/doc/source.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/tutorial_conftest.rst` & `ragger-1.9.2/doc/tutorial_conftest.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/tutorial_installation.rst` & `ragger-1.9.2/doc/tutorial_installation.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/doc/tutorial_screen.rst` & `ragger-1.9.2/doc/tutorial_screen.rst`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/setup.cfg` & `ragger-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/__init__.py` & `ragger-1.9.2/src/ragger/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/__init__.py` & `ragger-1.9.2/src/ragger/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/interface.py` & `ragger-1.9.2/src/ragger/backend/interface.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/ledgercomm.py` & `ragger-1.9.2/src/ragger/backend/ledgercomm.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/ledgerwallet.py` & `ragger-1.9.2/src/ragger/backend/ledgerwallet.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/physical_backend.py` & `ragger-1.9.2/src/ragger/backend/physical_backend.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/speculos.py` & `ragger-1.9.2/src/ragger/backend/speculos.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/backend/stub.py` & `ragger-1.9.2/src/ragger/backend/stub.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/bip/__init__.py` & `ragger-1.9.2/src/ragger/bip/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/bip/path.py` & `ragger-1.9.2/src/ragger/bip/path.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/bip/seed.py` & `ragger-1.9.2/src/ragger/bip/seed.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/conftest/base_conftest.py` & `ragger-1.9.2/src/ragger/conftest/base_conftest.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/conftest/configuration.py` & `ragger-1.9.2/src/ragger/conftest/configuration.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/error.py` & `ragger-1.9.2/src/ragger/error.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/__init__.py` & `ragger-1.9.2/src/ragger/firmware/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/stax/__init__.py` & `ragger-1.9.2/src/ragger/firmware/stax/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/stax/layouts.py` & `ragger-1.9.2/src/ragger/firmware/stax/layouts.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/stax/positions.py` & `ragger-1.9.2/src/ragger/firmware/stax/positions.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/stax/screen.py` & `ragger-1.9.2/src/ragger/firmware/stax/screen.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/stax/use_cases.py` & `ragger-1.9.2/src/ragger/firmware/stax/use_cases.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/structs.py` & `ragger-1.9.2/src/ragger/firmware/structs.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/firmware/versions.py` & `ragger-1.9.2/src/ragger/firmware/versions.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/__init__.py` & `ragger-1.9.2/src/ragger/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanos_body.png` & `ragger-1.9.2/src/ragger/gui/assets/nanos_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanos_leftbutton.png` & `ragger-1.9.2/src/ragger/gui/assets/nanos_leftbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanos_rightbutton.png` & `ragger-1.9.2/src/ragger/gui/assets/nanos_rightbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanosp_body.png` & `ragger-1.9.2/src/ragger/gui/assets/nanosp_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanosp_leftbutton.png` & `ragger-1.9.2/src/ragger/gui/assets/nanosp_leftbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanosp_rightbutton.png` & `ragger-1.9.2/src/ragger/gui/assets/nanosp_rightbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanox_body.png` & `ragger-1.9.2/src/ragger/gui/assets/nanox_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanox_leftbutton.png` & `ragger-1.9.2/src/ragger/gui/assets/nanox_leftbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/nanox_rightbutton.png` & `ragger-1.9.2/src/ragger/gui/assets/nanox_rightbutton.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/stax_body.png` & `ragger-1.9.2/src/ragger/gui/assets/stax_body.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/assets/touch_action.png` & `ragger-1.9.2/src/ragger/gui/assets/touch_action.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/interface.py` & `ragger-1.9.2/src/ragger/gui/interface.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/gui/process.py` & `ragger-1.9.2/src/ragger/gui/process.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/logger.py` & `ragger-1.9.2/src/ragger/logger.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/navigator/__init__.py` & `ragger-1.9.2/src/ragger/navigator/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/navigator/instruction.py` & `ragger-1.9.2/src/ragger/navigator/instruction.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/navigator/nano_navigator.py` & `ragger-1.9.2/src/ragger/navigator/nano_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/navigator/navigator.py` & `ragger-1.9.2/src/ragger/navigator/navigator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
 """
 from abc import ABC
 from pathlib import Path
+from tempfile import NamedTemporaryFile
 from time import time
 from typing import Callable, Dict, List, Optional, Union
 
 from ragger.backend import BackendInterface, SpeculosBackend
 from ragger.firmware import Firmware
 from ragger.utils import Crop
 
@@ -140,28 +141,60 @@
                          test_case_name: Optional[Path] = None,
                          snap_idx: int = 0) -> None:
         if isinstance(instruction, NavInsID):
             instruction = NavIns(instruction)
         if instruction.id not in self._callbacks:
             raise NotImplementedError(f"No callback registered for instruction ID {instruction.id}")
 
-        # Call instruction callback
-        self._callbacks[instruction.id](*instruction.args, **instruction.kwargs)
+        if instruction.id == NavInsID.USE_CASE_REVIEW_CONFIRM:
+            # Specific handling due to the fact that the screen is updated multiple
+            # time with a progress bar during this instruction callback execution.
+            # Indeed, this progress bar implies a screen change with previous screen
+            # content known by the backend.
+            # Therefore simply calling wait_for_screen_change() here will result in
+            # race issues.
+            # That's why we are first backuping the screen content in a temp file.
+            # This screen content is then used to check if the screen changed enough,
+            # e.g. with cropping the progress bar from the screen.
+            with NamedTemporaryFile(suffix='.png') as tmp:
+                tmp_file = Path(tmp.name)
+                # Backup screen content before instruction in tmp file
+                self._backend.compare_screen_with_snapshot(tmp_file,
+                                                           tmp_snap_path=tmp_file,
+                                                           golden_run=True)
+
+                # Call instruction callback
+                self._callbacks[instruction.id](*instruction.args, **instruction.kwargs)
+
+                # Wait for screen change unless explicitly specify otherwise
+                if wait_for_screen_change:
+                    # Compare to previous backup file without considering the bottom
+                    # which holds the progress bar.
+                    cropping = Crop(lower=220)
+                    endtime = time() + timeout
+                    while True:
+                        self._backend.wait_for_screen_change(endtime - time())
+                        if not self._backend.compare_screen_with_snapshot(tmp_file, cropping):
+                            break
 
-        # Wait for screen change unless explicitly specify otherwise
-        if wait_for_screen_change:
-            if instruction.id in [
-                    NavInsID.WAIT_FOR_SCREEN_CHANGE, NavInsID.WAIT_FOR_HOME_SCREEN,
-                    NavInsID.WAIT_FOR_TEXT_ON_SCREEN, NavInsID.WAIT_FOR_TEXT_NOT_ON_SCREEN
-            ]:
-                # Function wait_for_screen_change() is already called during
-                # instruction callback execution above.
-                pass
-            else:
-                self._backend.wait_for_screen_change(timeout)
+        else:
+            # Call instruction callback
+            self._callbacks[instruction.id](*instruction.args, **instruction.kwargs)
+
+            # Wait for screen change unless explicitly specify otherwise
+            if wait_for_screen_change:
+                if instruction.id in [
+                        NavInsID.WAIT_FOR_SCREEN_CHANGE, NavInsID.WAIT_FOR_HOME_SCREEN,
+                        NavInsID.WAIT_FOR_TEXT_ON_SCREEN, NavInsID.WAIT_FOR_TEXT_NOT_ON_SCREEN
+                ]:
+                    # Function wait_for_screen_change() is already called during
+                    # instruction callback execution above.
+                    pass
+                else:
+                    self._backend.wait_for_screen_change(timeout)
 
         # Compare snap with golden reference
         if path and test_case_name:
             if snap_idx == 0:
                 snaps_tmp_path = self._init_snaps_temp_dir(path, test_case_name)
                 snaps_golden_path = self._check_snaps_dir_path(path, test_case_name, True)
             else:
```

### Comparing `ragger-1.9.1/src/ragger/navigator/stax_navigator.py` & `ragger-1.9.2/src/ragger/navigator/stax_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/utils/__init__.py` & `ragger-1.9.2/src/ragger/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/utils/misc.py` & `ragger-1.9.2/src/ragger/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/utils/packing.py` & `ragger-1.9.2/src/ragger/utils/packing.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger/utils/structs.py` & `ragger-1.9.2/src/ragger/utils/structs.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/src/ragger.egg-info/PKG-INFO` & `ragger-1.9.2/src/ragger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragger
-Version: 1.9.1
+Version: 1.9.2
 Summary: Testing framework using Speculos and LedgerComm as backends
 Home-page: https://github.com/LedgerHQ/ragger
 Author: Ledger
 Author-email: hello@ledger.fr
 Project-URL: Bug Tracker, https://github.com/LedgerHQ/ragger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ragger-1.9.1/src/ragger.egg-info/SOURCES.txt` & `ragger-1.9.2/src/ragger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/template/conftest.py` & `ragger-1.9.2/template/conftest.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/template/usage.md` & `ragger-1.9.2/template/usage.md`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/conftest.py` & `ragger-1.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/functional/backend/test_speculos.py` & `ragger-1.9.2/tests/functional/backend/test_speculos.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/functional/navigator/test_navigator.py` & `ragger-1.9.2/tests/functional/navigator/test_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/functional/test_boilerplate.py` & `ragger-1.9.2/tests/functional/test_boilerplate.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00000.png` & `ragger-1.9.2/tests/snapshots/stax/waiting_screen/00000.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00001.png` & `ragger-1.9.2/tests/snapshots/stax/waiting_screen/00001.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00002.png` & `ragger-1.9.2/tests/snapshots/stax/waiting_screen/00002.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00003.png` & `ragger-1.9.2/tests/snapshots/stax/waiting_screen/00003.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/snapshots/stax/waiting_screen/00004.png` & `ragger-1.9.2/tests/snapshots/stax/waiting_screen/00004.png`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/stubs.py` & `ragger-1.9.2/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/backend/test_interface.py` & `ragger-1.9.2/tests/unit/backend/test_interface.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/backend/test_ledgercomm.py` & `ragger-1.9.2/tests/unit/backend/test_ledgercomm.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/backend/test_ledgerwallet.py` & `ragger-1.9.2/tests/unit/backend/test_ledgerwallet.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/backend/test_physical_backend.py` & `ragger-1.9.2/tests/unit/backend/test_physical_backend.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/backend/test_speculos.py` & `ragger-1.9.2/tests/unit/backend/test_speculos.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/bip/test_path.py` & `ragger-1.9.2/tests/unit/bip/test_path.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/bip/test_seed.py` & `ragger-1.9.2/tests/unit/bip/test_seed.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/firmware/stax/test_layouts__Layout.py` & `ragger-1.9.2/tests/unit/firmware/stax/test_layouts__Layout.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/firmware/stax/test_screen_FullScreen.py` & `ragger-1.9.2/tests/unit/firmware/stax/test_screen_FullScreen.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/firmware/stax/test_screen_MetaScreen.py` & `ragger-1.9.2/tests/unit/firmware/stax/test_screen_MetaScreen.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/firmware/test_structs_Firmware.py` & `ragger-1.9.2/tests/unit/firmware/test_structs_Firmware.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/firmware/test_versions_VersionManager.py` & `ragger-1.9.2/tests/unit/firmware/test_versions_VersionManager.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/navigator/test_navigator.py` & `ragger-1.9.2/tests/unit/navigator/test_navigator.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/utils/test_misc.py` & `ragger-1.9.2/tests/unit/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `ragger-1.9.1/tests/unit/utils/test_packing.py` & `ragger-1.9.2/tests/unit/utils/test_packing.py`

 * *Files identical despite different names*

