# Comparing `tmp/metar-taf-parser-mivek-1.6.3.tar.gz` & `tmp/metar-taf-parser-mivek-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/python-metar-taf-parser/python-metar-taf-parser/dist/.tmp-xyh5a6w0/metar-taf-parser-mivek-1.6.3.tar", last modified: Sun Mar 12 16:43:14 2023, max compression
+gzip compressed data, was "/home/runner/work/python-metar-taf-parser/python-metar-taf-parser/dist/.tmp-8bkbmm03/metar-taf-parser-mivek-1.6.4.tar", last modified: Fri Jun 23 21:48:30 2023, max compression
```

## Comparing `metar-taf-parser-mivek-1.6.3.tar` & `metar-taf-parser-mivek-1.6.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/metar.py
--rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/remark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/taf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/zh-CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/zh-CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser/parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-12 16:43:01.000000 metar-taf-parser-mivek-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-12 16:43:14.000000 metar-taf-parser-mivek-1.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/metar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26943 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/remark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/taf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11604 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16311 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/zh-CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/zh-CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11595 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21131 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser/parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 21:48:19.000000 metar-taf-parser-mivek-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-23 21:48:30.000000 metar-taf-parser-mivek-1.6.4/setup.cfg
```

### Comparing `metar-taf-parser-mivek-1.6.3/CHANGELOG.md` & `metar-taf-parser-mivek-1.6.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log 
 
+## [1.6.4] - 2023-06-TBD
+
+### Fixed
+
+- Parsing of `TAF` with stations starting by `FM`.
+
 ## [1.6.3] - 2023-03-12
 
 ### Fixed
 
 - Parsing of token `0000KT` no longer causes an error.
 
 ## [1.6.2] - 2023-01-29
```

### Comparing `metar-taf-parser-mivek-1.6.3/LICENSE` & `metar-taf-parser-mivek-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/PKG-INFO` & `metar-taf-parser-mivek-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar-taf-parser-mivek
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python project parsing metar and taf message
 Home-page: https://github.com/mivek/python-metar-taf-parser
 Author: Jean-Kevin KPADEY
 Author-email: jeankevin.kpadey@gmail.com
 Project-URL: Bug Tracker, https://github.com/mivek/python-metar-taf-parser/issues
 Keywords: metar,taf,parser,icao,airport
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metar-taf-parser-mivek-1.6.3/README.md` & `metar-taf-parser-mivek-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/common.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/common.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/metar.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/metar.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/remark.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/remark.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/command/taf.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/command/taf.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/converter.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/converter.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/commons/i18n.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/commons/i18n.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/de/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/en/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/es/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/es/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/it/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/messages.pot` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/locale/zh-CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/model/enum.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/model/enum.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/model/model.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/model/model.py`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser/parser/parser.py` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser/parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         """
         Format the message as a multiple line code so each line can be parsed
         :param taf_code: The base message
         :return: a list of string representing the lines of the message.
         """
         single_line = taf_code.replace('\n', ' ')
         clean_line = re.sub(r'\s{2,}', ' ', single_line)
-        lines = re.sub(r'\s(PROB\d{2}\sTEMPO|TEMPO|INTER|BECMG|FM|PROB)', '\n\g<1>', clean_line).splitlines()
+        lines = re.sub(r'\s(PROB\d{2}\sTEMPO|TEMPO|INTER|BECMG|FM(?![A-Z]{2}\s)|PROB)', '\n\g<1>', clean_line).splitlines()
         lines_token = [self.tokenize(line) for line in lines]
 
         if len(lines_token) > 1:
             last_line = lines_token[len(lines) - 1]
             temperatures = list(filter(lambda x: x.startswith(TAFParser.TX) or x.startswith(TAFParser.TN), last_line))
 
             if temperatures:
```

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/PKG-INFO` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar-taf-parser-mivek
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python project parsing metar and taf message
 Home-page: https://github.com/mivek/python-metar-taf-parser
 Author: Jean-Kevin KPADEY
 Author-email: jeankevin.kpadey@gmail.com
 Project-URL: Bug Tracker, https://github.com/mivek/python-metar-taf-parser/issues
 Keywords: metar,taf,parser,icao,airport
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metar-taf-parser-mivek-1.6.3/metar_taf_parser_mivek.egg-info/SOURCES.txt` & `metar-taf-parser-mivek-1.6.4/metar_taf_parser_mivek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metar-taf-parser-mivek-1.6.3/setup.cfg` & `metar-taf-parser-mivek-1.6.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = metar-taf-parser-mivek
-version = 1.6.3
+version = 1.6.4
 author = Jean-Kevin KPADEY
 author_email = jeankevin.kpadey@gmail.com
 description = Python project parsing metar and taf message
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mivek/python-metar-taf-parser
 project_urls =
```

